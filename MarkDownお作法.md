# Markdownの基本的な機能
基本的に改行する際は、列の最後に半角スペース2つ入れる必要があるが、後述する拡張を入れることで
改行がそのまま認識されるようになる。

また、htmlコードは自由に入れることが可能であるが、個人的にはあんま入れたくないかなーといった感じがする。入れ始めたら、`<br>`とか乱用しそうだから...
```
それでは、いってみよー
```
# 見出し系

# 見出し1
## 見出し2
### 見出し3
###### 見出し6

# 強調表示

*Italic*  
**イタリック**  

# 取り消し

~~取り消し線~~  

# リスト表示

* Item1
  * Item2
    * Item3

- 項目  
このように、リストアイテムの下の文章は  
インデントが自動で付く

1. アイテム
1. 数字は1のままでも、自動でナンバリングされる

# 引用文

>引用文はこんな感じ  
>やはり改行は、半角スペース２ついれないとされない。
>>頑張っても、vscodeでは上に余白を入れられない。。

# コードを書く時は

`インラインコード`

複数行にわたる場合は

`これを3つ打ったもの`で挟む。
ここでやっちゃうと、Qittaの都合上問題あるので、
個人で試してみてね

# 表形式の表示

| Left align | Right align | Center align |
|:-----------|------------:|:------------:|
| This       |        This |     This     |
| column     |      column |    column    |
| will       |        will |     will     |
| be         |          be |      be      |
| left       |       right |    center    |
| aligned    |     aligned |   aligned    |



| これが | グラフ | ちょっと書くのダルい？ |
|:-----:|--------|----------------------|
|そんな|感じの|印象です。|
|横幅ずーーーーーーっと広げてくと、勝手に広がります。| なるほど| なぁ

# 線を引く

---
こんな感じに
***
`<hr>`的なのが引ける。記号の間にスペースがあっても問題ない
* * *

# URL

[Qiita](http://qiita.com/)  
[Google](https://www.google.co.jp/)  
<http://qiita.com>

# 注釈

今日はいい天気[^1]  
注釈はなぜか一番下に表示される[^test]  
VScodeでは使えないようだ。。

# 数式

数式は、拡張機能「Markdown Preview Enhanced」を入れることで書くことが可能になる。
数がありすぎるので、ここでは代表的なものだけ。
ちなみにすべて[こちら](http://www.eng.niigata-u.ac.jp/~nomoto/download/mathjax.pdf)を参考にした。
まだまだあるのも、[こちら](http://www.eng.niigata-u.ac.jp/~nomoto/download/mathjax.pdf)を参考にされたし。

***
## 一次方程式

一次方程式 \(ax+b=0\) の解は
\[
x = -\frac{b}{a}
\]
です。

***
## 二次方程式

二次方程式 \(ax^{2}+bx+c=0\) の解は
\[
x = \frac{-b\pm\sqrt{b^{2}-4ac}}{2a} 
\]
です。

***
## シグマ
\[
\sum_{k=1}^{n} a_{k} = a_{1} + a_{2} + \dots + a_{n}
\]

***
## ガウス積分
\[
\int_{-\infty}^{\infty} e^{-x^{2}} \, dx = \sqrt{\pi}
\]

*** 
## 関数 f(x) の導関数

関数 \(f(x)\) の導関数は
\[
f(x) = \lim_{\Delta x \to 0} \frac{ f(x+\Delta x) - f(x) }{\Delta x}
\]
である。

***
## サイン、コサイン、タンジェント

\[
\int \tan\theta \, d\theta = \int \frac{\sin\theta}{\cos\theta} \, d\theta
= -\log |\cos\theta| + C
\]

***
## 行列

\(n \times n\) 行列
\[
A =
\begin{pmatrix}
a_{11} & a_{12} & \ldots & a_{1n} \\
a_{21} & a_{22} & \ldots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & \ldots & a_{nn}
\end{pmatrix}
\]
が逆行列 \(A^{-1}\) をもつための必要十分条件は、\(\det A \neq 0\) である。


####「Markdown All in One」と「Markdown Preview Enhanced」は入れるべし
入れることで得られるメリット
* 数式が使える
* キーボードショートカットが使える
* リスト表示が、Enterキーを打つだけで自動で続く
* 改行に、スペース2つを入れる必要がない
* PDFやHTMLでの出力が容易
* CSSで、規定の文字サイズ等を変更することもできる
* 整形も容易
* グラフとかもかけるらしい<http://yohshiy.blog.fc2.com/blog-category-22.html>けどよくわかってない

キーボードショートカット
| ショートカットキー        | 対応する表示形式       |
| :--------------: | :------------------: |
| Crtl - b         | 強調表示（ `** **`） |
| Crtl - i         | italic表示（ `* *`） |
| Ctrl - shift - ] | 見出しを増やす（`#`）    |
| Ctrl - shift - [ | 見出しを減らす（`#`）    |

<img width="数値" alt="代替テキスト" src="URL">