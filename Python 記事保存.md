# Pythonでのローカル環境構築について
LINE APIを利用して、AWS API GateWay~Lambda〜S3への構築を行う際に、LambdaにPythonを利用してコードを書こうと思い立ち、まず環境構築からというところで躓きがあったので記述をしていきます。

---

## 構築前の状態（前提条件）
Macを利用しているので標準でPythonがインストールされていますが、バージョンが古いので、こちらを「3系」を利用できる様にしていきます。
```
inamurateppei@mbp projects % python --version
Python 2.7.16
```

先に記述するとOSを「**Catalina**」→「**BigSur**」にしたため、Pythonの最新バージョンをGetすることが出来ませんでした。
画像

ちなみに「**Homebrew**」はRubyを学習したのでインストールが済んでいる状態です。
```
inamurateppei@mbp projects % brew -v
Homebrew 3.1.7
Homebrew/homebrew-core (git revision 0e20a3258c; last commit 2021-05-16)
```
「**Pyenv(パイエンブ)**」ツールを利用してPythonをインストールする方法を考えて、状態を確認してみます。
下記のコマンドの通り、インストールされていないことが確認できます。
```
inamurateppei@mbp projects % pyenv -v
zsh: command not found: pyenv
```
___
## Pyenv（パイエンブ）インストール
```
inamurateppei@mbp projects % brew install pyenv
Updating Homebrew...
--- 省略 ---
```
ちゃんとインストールされているか確認してみます
```
inamurateppei@mbp projects % pyenv -v
pyenv 1.2.27
```
---
## パスを通す
```
inamurateppei@mbp projects % echo $SHELL
/bin/zsh
```
```
inamurateppei@mbp projects % echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
inamurateppei@mbp projects % echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
inamurateppei@mbp projects % echo 'eval "$(pyenv init -)"' >> ~/.zshrc
inamurateppei@mbp projects % source ~/.zshrc
```
---
## Pythonのインストール
インストールしたPyenvを用いてPythonをインストールしていきます
```
inamurateppei@mbp projects % pyenv install --list
Available versions:
  2.1.3
--- 略 --- 
```
---
## ※ここで躓く！！
なんか「**xcrun**」となるもののパスが見当たらないみたい。
```
inamurateppei@mbp projects % pyenv install 3.9.0
python-build: use openssl from homebrew
python-build: use readline from homebrew
--- 中略 ---
checking whether the C compiler works... no
configure: error: in `/var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522115358.28038/Python-3.6.5':
configure: error: C compiler cannot create executables
See `config.log' for more details
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun
```
調べてみると、Xcodeの開発者ツールが見当たらなくなってしまっていることが原因とのことで、Mac OSをアップデートした時にあるあるネタということが分かる。

---

## 対処方法
下記のコマンドで「**xcode**」をインストールし直す
```
inamurateppei@mbp % xcode-select --install
xcode-select: note: install requested for command line developer tools
```
---
## ※再び躓く！！
Buildが出来ないと出てしまっている。とりあえずググる。
```
inamurateppei@mbp % pyenv install 3.9.0
python-build: use openssl from homebrew
python-build: use readline from homebrew
--- 中略 ---
BUILD FAILED (OS X 11.2.3 using python-build 20180424)
--- 中略 ---
Last 10 log lines:
./Modules/posixmodule.c:8210:15: error: implicit declaration of function 'sendfile' is invalid in C99 [-Werror,-Wimplicit-function-declaration]
        ret = sendfile(in, out, offset, &sbytes, &sf, flags);
              ^
./Modules/posixmodule.c:10432:5: warning: code will never be executed [-Wunreachable-code]
    Py_FatalError("abort() called from Python code didn't abort!");
    ^~~~~~~~~~~~~
1 warning and 1 error generated.
make: *** [Modules/posixmodule.o] Error 1
make: *** Waiting for unfinished jobs....
1 warning generated.
```
---
## 対処方法
1.**update**でHomebrewの各パッケージの情報をアップデート  
2.**upgrade**でパッケージの更新  
3.Zlibを利用するためインストールする  
4.pythonのバージョンを切り替える  
5.バージョン3.9.0をインストール
```
inamurateppei@mbp ~ % brew update
inamurateppei@mbp ~ % brew upgrade
inamurateppei@mbp ~ % brew install pyenv zlib bzip2 readline
inamurateppei@mbp ~ % eval "$(pyenv init -)"
inamurateppei@mbp ~ % CPPFLAGS="-I$(brew --prefix openssl)/include -I$(brew --prefix bzip2)/include -I$(brew --prefix readline)/include -I$(brew --prefix zlib)/include" LDFLAGS="-L$(brew --prefix openssl)/lib -L$(brew --prefix readline)/lib -L$(brew --prefix zlib)/lib -L$(brew --prefix bzip2)/lib" pyenv install 3.9.0
```
---
## 結果
```
inamurateppei@mbp ~ % pyenv versions
* system (set by /Users/inamurateppei/.pyenv/version)
  3.9.0
inamurateppei@mbp ~ % pyenv global 3.9.0
```
---
## バージョンを確認する
zshにパスを通して環境構築終了
```
inamurateppei@mbp ~ % python --version
Python 2.7.16
inamurateppei@mbp ~ % pyenv global 3.9.0
inamurateppei@mbp ~ % zsh -l
inamurateppei@mbp ~ % python --version
Python 3.9.0
```
---
## さっそく次回からLambdaを利用して構築をしていきたいと思います。