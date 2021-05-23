
```
inamurateppei@mbp projects % python --version
Python 2.7.16
```
```
inamurateppei@mbp projects % brew -v
Homebrew 3.1.7
Homebrew/homebrew-core (git revision 0e20a3258c; last commit 2021-05-16)
```
```
inamurateppei@mbp projects % pyenv -v
zsh: command not found: pyenv
```
```
inamurateppei@mbp projects % brew install pyenv
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 3 taps (heroku/brew, homebrew/core and homebrew/services).
==> New Formulae
clazy           erlang@23       gitwatch        grepip          marp-cli        nomino          parquet-cli     tbb@2020
ehco            gitbackup       gradle@6        ipinfo-cli      neovim-remote   opensearch      php-cs-fixer@2
==> Updated Formulae
Updated 407 formulae.
==> Deleted Formulae
osquery
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun

==> Downloading https://ghcr.io/v2/homebrew/core/m4/manifests/1.4.18-1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/m4/blobs/sha256:0df9083b268f76a3cda0c9f0d2ce84b51d21a8618d578740646fb615b00c7e
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:0df9083b268f76a3cda0c9f0d2ce84b51d21a8618d
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/autoconf/manifests/2.71
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/autoconf/blobs/sha256:0aa64f171bac19ce6ac0c0ca697f30658db78cf175550dfde3dbda90
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:0aa64f171bac19ce6ac0c0ca697f30658db78cf175
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pyenv/manifests/1.2.27
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pyenv/blobs/sha256:78939e92d2be55add6503458fa96059e36bb9e37e5b9fb72e724d1813b2
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:78939e92d2be55add6503458fa96059e36bb9e37e5
######################################################################## 100.0%
==> Installing dependencies for pyenv: m4 and autoconf
==> Installing pyenv dependency: m4
==> Pouring m4--1.4.18.big_sur.bottle.1.tar.gz
==> Caveats
m4 is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have m4 first in your PATH, run:
  echo 'export PATH="/usr/local/opt/m4/bin:$PATH"' >> ~/.zshrc

==> Summary
🍺  /usr/local/Cellar/m4/1.4.18: 13 files, 672.3KB
==> Installing pyenv dependency: autoconf
==> Pouring autoconf--2.71.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/autoconf/2.71: 71 files, 3.2MB
==> Installing pyenv
==> Pouring pyenv--1.2.27.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/pyenv/1.2.27: 750 files, 2.6MB
==> Upgrading 1 dependent:
ruby-build 20201210 -> 20210510
==> Upgrading ruby-build 20201210 -> 20210510 
==> Downloading https://ghcr.io/v2/homebrew/core/ruby-build/manifests/20210510
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ruby-build/blobs/sha256:92c2ec2f10038f644c8d8c0adcc123170d384f72951570724f0b2c
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:92c2ec2f10038f644c8d8c0adcc123170d384f7295
######################################################################## 100.0%
==> Pouring ruby-build--20210510.all.bottle.tar.gz
==> Caveats
ruby-build installs a non-Homebrew OpenSSL for each Ruby version installed and these are never upgraded.

To link Rubies to Homebrew's OpenSSL 1.1 (which is upgraded) add the following
to your ~/.zshrc:
  export RUBY_CONFIGURE_OPTS="--with-openssl-dir=$(brew --prefix openssl@1.1)"

Note: this may interfere with building old versions of Ruby (e.g <2.4) that use
OpenSSL <1.1.
==> Summary
🍺  /usr/local/Cellar/ruby-build/20210510: 530 files, 264.4KB
Removing: /usr/local/Cellar/ruby-build/20201210... (514 files, 256.9KB)
==> Checking for dependents of upgraded formulae...
==> No broken dependents found!
==> Caveats
==> m4
m4 is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have m4 first in your PATH, run:
  echo 'export PATH="/usr/local/opt/m4/bin:$PATH"' >> ~/.zshrc

==> ruby-build
ruby-build installs a non-Homebrew OpenSSL for each Ruby version installed and these are never upgraded.

To link Rubies to Homebrew's OpenSSL 1.1 (which is upgraded) add the following
to your ~/.zshrc:
  export RUBY_CONFIGURE_OPTS="--with-openssl-dir=$(brew --prefix openssl@1.1)"

Note: this may interfere with building old versions of Ruby (e.g <2.4) that use
OpenSSL <1.1.
inamurateppei@mbp projects % pyenv -v
pyenv 1.2.27
inamurateppei@mbp projects % exho $SHELL
zsh: command not found: exho
inamurateppei@mbp projects % echo $SHELL
/bin/zsh
inamurateppei@mbp projects % echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
inamurateppei@mbp projects % echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
inamurateppei@mbp projects % echo 'eval "$(pyenv init -)"' >> ~/.zshrc

inamurateppei@mbp projects % source ~/.zshrc
inamurateppei@mbp projects % exho $SHELL                                           
zsh: command not found: exho
inamurateppei@mbp projects % echo $SHELL                                           
/bin/zsh
inamurateppei@mbp projects % echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc   
inamurateppei@mbp projects % echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
inamurateppei@mbp projects % echo 'eval "$(pyenv init -)"' >> ~/.zshrc             
inamurateppei@mbp projects % source ~/.zshrc                                       
inamurateppei@mbp projects % echo $SHELL                                           
/bin/zsh
```
```
inamurateppei@mbp projects % pyenv install --list
Available versions:
  2.1.3
  2.2.3
  2.3.7
  2.4.0
  2.4.1
  2.4.2
  2.4.3
  2.4.4
  2.4.5
  2.4.6
  2.5.0
  2.5.1
  2.5.2
  2.5.3
  2.5.4
  2.5.5
  2.5.6
  2.6.6
  2.6.7
  2.6.8
  2.6.9
  2.7.0
  2.7-dev
  2.7.1
  2.7.2
  2.7.3
  2.7.4
  2.7.5
  2.7.6
  2.7.7
  2.7.8
  2.7.9
  2.7.10
  2.7.11
  2.7.12
  2.7.13
  2.7.14
  2.7.15
  2.7.16
  2.7.17
  2.7.18
  3.0.1
  3.1.0
  3.1.1
  3.1.2
  3.1.3
  3.1.4
  3.1.5
  3.2.0
  3.2.1
  3.2.2
  3.2.3
  3.2.4
  3.2.5
  3.2.6
  3.3.0
  3.3.1
  3.3.2
  3.3.3
  3.3.4
  3.3.5
  3.3.6
  3.3.7
  3.4.0
  3.4-dev
  3.4.1
  3.4.2
  3.4.3
  3.4.4
  3.4.5
  3.4.6
  3.4.7
  3.4.8
  3.4.9
  3.4.10
  3.5.0
  3.5-dev
  3.5.1
  3.5.2
  3.5.3
  3.5.4
  3.5.5
  3.5.6
  3.5.7
  3.5.8
  3.5.9
  3.5.10
  3.6.0
  3.6-dev
  3.6.1
  3.6.2
  3.6.3
  3.6.4
  3.6.5
  3.6.6
  3.6.7
  3.6.8
  3.6.9
  3.6.10
  3.6.11
  3.6.12
  3.6.13
  3.7.0
  3.7-dev
  3.7.1
  3.7.2
  3.7.3
  3.7.4
  3.7.5
  3.7.6
  3.7.7
  3.7.8
  3.7.9
  3.7.10
  3.8.0
  3.8-dev
  3.8.1
  3.8.2
  3.8.3
  3.8.4
  3.8.5
  3.8.6
  3.8.7
  3.8.8
  3.8.9
  3.9.0
  3.9-dev
  3.9.1
  3.9.2
  3.9.3
  3.9.4
  3.10.0a7
  3.10-dev
  activepython-2.7.14
  activepython-3.5.4
  activepython-3.6.0
  anaconda-1.4.0
  anaconda-1.5.0
  anaconda-1.5.1
  anaconda-1.6.0
  anaconda-1.6.1
  anaconda-1.7.0
  anaconda-1.8.0
  anaconda-1.9.0
  anaconda-1.9.1
  anaconda-1.9.2
  anaconda-2.0.0
  anaconda-2.0.1
  anaconda-2.1.0
  anaconda-2.2.0
  anaconda-2.3.0
  anaconda-2.4.0
  anaconda-4.0.0
  anaconda2-2.4.0
  anaconda2-2.4.1
  anaconda2-2.5.0
  anaconda2-4.0.0
  anaconda2-4.1.0
  anaconda2-4.1.1
  anaconda2-4.2.0
  anaconda2-4.3.0
  anaconda2-4.3.1
  anaconda2-4.4.0
  anaconda2-5.0.0
  anaconda2-5.0.1
  anaconda2-5.1.0
  anaconda2-5.2.0
  anaconda2-5.3.0
  anaconda2-5.3.1
  anaconda2-2018.12
  anaconda2-2019.03
  anaconda2-2019.07
  anaconda3-2.0.0
  anaconda3-2.0.1
  anaconda3-2.1.0
  anaconda3-2.2.0
  anaconda3-2.3.0
  anaconda3-2.4.0
  anaconda3-2.4.1
  anaconda3-2.5.0
  anaconda3-4.0.0
  anaconda3-4.1.0
  anaconda3-4.1.1
  anaconda3-4.2.0
  anaconda3-4.3.0
  anaconda3-4.3.1
  anaconda3-4.4.0
  anaconda3-5.0.0
  anaconda3-5.0.1
  anaconda3-5.1.0
  anaconda3-5.2.0
  anaconda3-5.3.0
  anaconda3-5.3.1
  anaconda3-2018.12
  anaconda3-2019.03
  anaconda3-2019.07
  anaconda3-2019.10
  anaconda3-2020.02
  anaconda3-2020.07
  anaconda3-2020.11
  graalpython-20.1.0
  graalpython-20.2.0
  graalpython-20.3.0
  graalpython-21.0.0
  graalpython-21.1.0
  ironpython-dev
  ironpython-2.7.4
  ironpython-2.7.5
  ironpython-2.7.6.3
  ironpython-2.7.7
  jython-dev
  jython-2.5.0
  jython-2.5-dev
  jython-2.5.1
  jython-2.5.2
  jython-2.5.3
  jython-2.5.4-rc1
  jython-2.7.0
  jython-2.7.1
  jython-2.7.2
  micropython-dev
  micropython-1.9.3
  micropython-1.9.4
  micropython-1.10
  micropython-1.11
  micropython-1.12
  micropython-1.13
  micropython-1.14
  miniconda-latest
  miniconda-2.2.2
  miniconda-3.0.0
  miniconda-3.0.4
  miniconda-3.0.5
  miniconda-3.3.0
  miniconda-3.4.2
  miniconda-3.7.0
  miniconda-3.8.3
  miniconda-3.9.1
  miniconda-3.10.1
  miniconda-3.16.0
  miniconda-3.18.3
  miniconda2-latest
  miniconda2-3.18.3
  miniconda2-3.19.0
  miniconda2-4.0.5
  miniconda2-4.1.11
  miniconda2-4.3.14
  miniconda2-4.3.21
  miniconda2-4.3.27
  miniconda2-4.3.30
  miniconda2-4.3.31
  miniconda2-4.4.10
  miniconda2-4.5.1
  miniconda2-4.5.4
  miniconda2-4.5.11
  miniconda2-4.5.12
  miniconda2-4.6.14
  miniconda2-4.7.10
  miniconda2-4.7.12
  miniconda3-latest
  miniconda3-2.2.2
  miniconda3-3.0.0
  miniconda3-3.0.4
  miniconda3-3.0.5
  miniconda3-3.3.0
  miniconda3-3.4.2
  miniconda3-3.7.0
  miniconda3-3.7-4.8.2
  miniconda3-3.7-4.8.3
  miniconda3-3.7-4.9.2
  miniconda3-3.8.3
  miniconda3-3.8-4.8.2
  miniconda3-3.8-4.8.3
  miniconda3-3.8-4.9.2
  miniconda3-3.9.1
  miniconda3-3.9-4.9.2
  miniconda3-3.10.1
  miniconda3-3.16.0
  miniconda3-3.18.3
  miniconda3-3.19.0
  miniconda3-4.0.5
  miniconda3-4.1.11
  miniconda3-4.2.12
  miniconda3-4.3.11
  miniconda3-4.3.14
  miniconda3-4.3.21
  miniconda3-4.3.27
  miniconda3-4.3.30
  miniconda3-4.3.31
  miniconda3-4.4.10
  miniconda3-4.5.1
  miniconda3-4.5.4
  miniconda3-4.5.11
  miniconda3-4.5.12
  miniconda3-4.6.14
  miniconda3-4.7.10
  miniconda3-4.7.12
  miniforge3-4.9.2
  miniforge3-4.10
  pypy-c-jit-latest
  pypy-dev
  pypy-stm-2.3
  pypy-stm-2.5.1
  pypy-1.5-src
  pypy-1.6
  pypy-1.7
  pypy-1.8
  pypy-1.9
  pypy-2.0-src
  pypy-2.0
  pypy-2.0.1-src
  pypy-2.0.1
  pypy-2.0.2-src
  pypy-2.0.2
  pypy-2.1-src
  pypy-2.1
  pypy-2.2-src
  pypy-2.2
  pypy-2.2.1-src
  pypy-2.2.1
  pypy-2.3-src
  pypy-2.3
  pypy-2.3.1-src
  pypy-2.3.1
  pypy-2.4.0-src
  pypy-2.4.0
  pypy-2.5.0-src
  pypy-2.5.0
  pypy-2.5.1-src
  pypy-2.5.1
  pypy-2.6.0-src
  pypy-2.6.0
  pypy-2.6.1-src
  pypy-2.6.1
  pypy-4.0.0-src
  pypy-4.0.0
  pypy-4.0.1-src
  pypy-4.0.1
  pypy-5.0.0-src
  pypy-5.0.0
  pypy-5.0.1-src
  pypy-5.0.1
  pypy-5.1-src
  pypy-5.1
  pypy-5.1.1-src
  pypy-5.1.1
  pypy-5.3-src
  pypy-5.3
  pypy-5.3.1-src
  pypy-5.3.1
  pypy-5.4-src
  pypy-5.4
  pypy-5.4.1-src
  pypy-5.4.1
  pypy-5.6.0-src
  pypy-5.6.0
  pypy-5.7.0-src
  pypy-5.7.0
  pypy-5.7.1-src
  pypy-5.7.1
  pypy2-5.3-src
  pypy2-5.3
  pypy2-5.3.1-src
  pypy2-5.3.1
  pypy2-5.4-src
  pypy2-5.4
  pypy2-5.4.1-src
  pypy2-5.4.1
  pypy2-5.6.0-src
  pypy2-5.6.0
  pypy2-5.7.0-src
  pypy2-5.7.0
  pypy2-5.7.1-src
  pypy2-5.7.1
  pypy2.7-5.8.0-src
  pypy2.7-5.8.0
  pypy2.7-5.9.0-src
  pypy2.7-5.9.0
  pypy2.7-5.10.0-src
  pypy2.7-5.10.0
  pypy2.7-6.0.0-src
  pypy2.7-6.0.0
  pypy2.7-7.0.0-src
  pypy2.7-7.0.0
  pypy2.7-7.1.0-src
  pypy2.7-7.1.0
  pypy2.7-7.1.1-src
  pypy2.7-7.1.1
  pypy2.7-7.2.0-src
  pypy2.7-7.2.0
  pypy2.7-7.3.0-src
  pypy2.7-7.3.0
  pypy2.7-7.3.1-src
  pypy2.7-7.3.1
  pypy3-2.3.1-src
  pypy3-2.3.1
  pypy3-2.4.0-src
  pypy3-2.4.0
  pypy3.3-5.2-alpha1-src
  pypy3.3-5.2-alpha1
  pypy3.3-5.5-alpha-src
  pypy3.3-5.5-alpha
  pypy3.5-c-jit-latest
  pypy3.5-5.7-beta-src
  pypy3.5-5.7-beta
  pypy3.5-5.7.1-beta-src
  pypy3.5-5.7.1-beta
  pypy3.5-5.8.0-src
  pypy3.5-5.8.0
  pypy3.5-5.9.0-src
  pypy3.5-5.9.0
  pypy3.5-5.10.0-src
  pypy3.5-5.10.0
  pypy3.5-5.10.1-src
  pypy3.5-5.10.1
  pypy3.5-6.0.0-src
  pypy3.5-6.0.0
  pypy3.5-7.0.0-src
  pypy3.5-7.0.0
  pypy3.6-7.0.0-src
  pypy3.6-7.0.0
  pypy3.6-7.1.0-src
  pypy3.6-7.1.0
  pypy3.6-7.1.1-src
  pypy3.6-7.1.1
  pypy3.6-7.2.0-src
  pypy3.6-7.2.0
  pypy3.6-7.3.0-src
  pypy3.6-7.3.0
  pypy3.6-7.3.1-src
  pypy3.6-7.3.1
  pypy3.6-7.3.2-src
  pypy3.6-7.3.2
  pypy3.6-7.3.3-src
  pypy3.6-7.3.3
  pypy3.7-c-jit-latest
  pypy3.7-7.3.2-src
  pypy3.7-7.3.2
  pypy3.7-7.3.3-src
  pypy3.7-7.3.3
  pypy3.7-7.3.4
  pyston-0.5.1
  pyston-0.6.0
  pyston-0.6.1
  stackless-dev
  stackless-2.7-dev
  stackless-2.7.2
  stackless-2.7.3
  stackless-2.7.4
  stackless-2.7.5
  stackless-2.7.6
  stackless-2.7.7
  stackless-2.7.8
  stackless-2.7.9
  stackless-2.7.10
  stackless-2.7.11
  stackless-2.7.12
  stackless-2.7.14
  stackless-3.2.2
  stackless-3.2.5
  stackless-3.3.5
  stackless-3.3.7
  stackless-3.4-dev
  stackless-3.4.2
  stackless-3.4.7
  stackless-3.5.4
  stackless-3.7.5
```
```
inamurateppei@mbp projects % pyenv install 3.6.5
python-build: use openssl from homebrew
python-build: use readline from homebrew
Downloading Python-3.6.5.tar.xz...
-> https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tar.xz
Installing Python-3.6.5...
python-build: use readline from homebrew

BUILD FAILED (OS X 11.2.3 using python-build 20180424)

Inspect or clean up the working tree at /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522115358.28038
Results logged to /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522115358.28038.log

Last 10 log lines:
checking for --with-universal-archs... no
checking MACHDEP... darwin
checking for --without-gcc... no
checking for --with-icc... no
checking for gcc... clang
checking whether the C compiler works... no
configure: error: in `/var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522115358.28038/Python-3.6.5':
configure: error: C compiler cannot create executables
See `config.log' for more details
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun
```
inamurateppei@mbp projects % ls
F lesson mylesson		furima-31782			protospace-31782
HTML_CSS			getting-started			rad_app
JavaScript			hello_app			rails6_docker_template
active_hash_app			html_layout			rails_new
ajax_app			javascript_skillcheck		responsive
ajax_app2			linux				ruby
app_myapp_nareru		mini_image_app			ruby_application_training
app_nareru			mini_sns			samp
app_nareru_2			mini_talk_app			sample
boot_lesson			myapp				sample-app
bootstrap			myapp2				search_app
bprotospace-31782		myapp_tekagami_2.0.1		sql-curriculum
breadcrumb			mydocker			tagtweet
chat-app			myprof				tamesigiri
chat_app2			nareru				tasukigake
docker_lesson1			narerua				techcamp
donation_app			note				tekagami_1.0.1
drill_app			ourblog_error1			tekagami_2.0.0
error_pictweet2_10		ourblog_error2			tekagami_2.1.0
error_pictweet2_8		paiza.txt			terraform_ecs_deploy
error_pictweet2_9		payjp_app			todo
error_pictweet5_2		payjp_practice			todo2
error_pictweet5_3		photo_app			toy_app
error_pictweet5_4		picturs				training
error_pictweet5_6		pictweet			training_curriculum
error_pictweet5_7		pictweet2_app			try_webpacker
error_pictweet_rails6		pictweet3			tweet_app
exception_sample		pictweet4			wizard_app
first_app			progate				works
inamurateppei@mbp projects % cd ..
inamurateppei@mbp ~ % ls
Applications		Downloads		Movies			Public			matter
Creative Cloud Files	Dropbox			Music			Sinatra			projects
Desktop			IWwedding		MyVagrant		VirtualBox VMs		readme.md
Documents		Library			Pictures		create
inamurateppei@mbp ~ % cd matter
inamurateppei@mbp matter % ls
iwphoto
inamurateppei@mbp matter % cd iwphoto
inamurateppei@mbp iwphoto % rails s
Could not find erubis-2.7.0 in any of the sources
Run `bundle install` to install missing gems.
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Fetching erubis 2.7.0
Installing erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Fetching temple 0.8.2
Installing temple 0.8.2
Using tilt 2.0.10
Fetching haml 5.2.1
Installing haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29188-1e462ri.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % git checkout -b devise origin       
fatal: 'origin' is not a commit and a branch 'devise' cannot be created from it
inamurateppei@mbp iwphoto % git checkout -b master       
Switched to a new branch 'master'
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29311-1oggb9q.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % git pull origin main
hint: Pulling without specifying how to reconcile divergent branches is
hint: discouraged. You can squelch this message by running one of the following
hint: commands sometime before your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
From https://github.com/tetutetu214/PhotoApp
 * branch            main       -> FETCH_HEAD
Already up to date.
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29365-y8r1mg.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % git pull origin main         
hint: Pulling without specifying how to reconcile divergent branches is
hint: discouraged. You can squelch this message by running one of the following
hint: commands sometime before your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
From https://github.com/tetutetu214/PhotoApp
 * branch            main       -> FETCH_HEAD
Already up to date.
inamurateppei@mbp iwphoto % rails s
Could not find hamlit-2.15.0 in any of the sources
Run `bundle install` to install missing gems.
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29426-lj7e7f.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % gem install hamlit -v '2.15.0'
Building native extensions. This could take a while...
ERROR:  Error installing hamlit:
	ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r ./siteconf20210522-29450-15vqdvh.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for inspection.
Results logged to /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out
inamurateppei@mbp iwphoto % bundle install                
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29466-10xami4.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Gem::Ext::BuildError: ERROR: Failed to build gem native extension.

    current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
/Users/inamurateppei/.rbenv/versions/2.6.5/bin/ruby -I /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/site_ruby/2.6.0 -r
./siteconf20210522-29532-65207y.rb extconf.rb
creating Makefile

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR=" clean
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

current directory: /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0/ext/hamlit
make "DESTDIR="
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
/Library/Developer/CommandLineTools/usr/bin/xcrun

make failed, exit code 1

Gem files will remain installed in /Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/hamlit-2.15.0 for
inspection.
Results logged to
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/extensions/x86_64-darwin-19/2.6.0/hamlit-2.15.0/gem_make.out

An error occurred while installing hamlit (2.15.0), and Bundler cannot continue.
Make sure that `gem install hamlit -v '2.15.0' --source 'https://rubygems.org/'` succeeds before bundling.

In Gemfile:
  hamlit-rails was resolved to 0.2.3, which depends on
    hamlit
inamurateppei@mbp iwphoto % xcode-select --install
xcode-select: note: install requested for command line developer tools
inamurateppei@mbp iwphoto % bundle install
The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
Fetching gem metadata from https://rubygems.org/.........
Using rake 13.0.3
Using concurrent-ruby 1.1.8
Using i18n 1.8.10
Using minitest 5.14.4
Using thread_safe 0.3.6
Using tzinfo 1.2.9
Using zeitwerk 2.4.2
Using activesupport 6.0.3.4
Using builder 3.2.4
Using erubi 1.10.0
Using mini_portile2 2.5.1
Using racc 1.5.2
Using nokogiri 1.11.4 (x86_64-darwin)
Using rails-dom-testing 2.0.3
Using crass 1.0.6
Using loofah 2.9.1
Using rails-html-sanitizer 1.3.0
Using actionview 6.0.3.4
Using rack 2.2.3
Using rack-test 1.1.0
Using actionpack 6.0.3.4
Using nio4r 2.5.4
Using websocket-extensions 0.1.5
Using websocket-driver 0.7.3
Using actioncable 6.0.3.4
Using globalid 0.4.2
Using activejob 6.0.3.4
Using activemodel 6.0.3.4
Using activerecord 6.0.3.4
Using mimemagic 0.3.5
Using marcel 0.3.3
Using activestorage 6.0.3.4
Using mini_mime 1.0.2
Using mail 2.7.1
Using actionmailbox 6.0.3.4
Using actionmailer 6.0.3.4
Using actiontext 6.0.3.4
Using active_hash 3.1.0
Using public_suffix 4.0.6
Using addressable 2.7.0
Using ast 2.4.2
Using bcrypt 3.1.16
Using bindex 0.8.1
Using msgpack 1.3.3
Using bootsnap 1.5.1
Using bundler 2.1.4
Using byebug 11.1.3
Using regexp_parser 1.8.2
Using xpath 3.2.0
Using capybara 3.34.0
Using childprocess 3.0.0
Using coderay 1.1.3
Using orm_adapter 0.5.0
Using method_source 1.0.0
Using thor 1.1.0
Using railties 6.0.3.4
Using responders 3.0.1
Using warden 1.2.9
Using devise 4.8.0
Using diff-lcs 1.4.4
Using dotenv 2.7.6
Using dotenv-rails 2.7.6
Using erubis 2.7.0
Using factory_bot 6.2.0
Using factory_bot_rails 6.2.0
Using faker 2.18.0
Using ffi 1.14.2
Using temple 0.8.2
Using tilt 2.0.10
Using haml 5.2.1
Fetching hamlit 2.15.0
Installing hamlit 2.15.0 with native extensions
Fetching hamlit-rails 0.2.3
Installing hamlit-rails 0.2.3
Fetching sexp_processor 4.15.3
Installing sexp_processor 4.15.3
Fetching ruby_parser 3.16.0
Installing ruby_parser 3.16.0
Fetching html2haml 2.2.0
Installing html2haml 2.2.0
Using mini_magick 4.11.0
Using ruby-vips 2.1.2
Using image_processing 1.12.1
Using jbuilder 2.10.1
Using rb-fsevent 0.10.4
Using rb-inotify 0.10.1
Using listen 3.4.1
Using mysql2 0.5.3
Using parallel 1.20.1
Using parser 3.0.1.1
Using pry 0.14.1
Using pry-byebug 3.8.0
Using pry-rails 0.3.9
Using puma 4.3.7
Using rack-proxy 0.6.5
Using sprockets 4.0.2
Using sprockets-rails 3.2.2
Using rails 6.0.3.4
Using rails-i18n 6.0.0
Using rainbow 3.0.0
Using rexml 3.2.5
Using rspec-support 3.10.2
Using rspec-core 3.10.1
Using rspec-expectations 3.10.1
Using rspec-mocks 3.10.2
Using rspec-rails 4.0.2
Using rubocop-ast 1.5.0
Using ruby-progressbar 1.11.0
Using unicode-display_width 2.0.0
Using rubocop 1.14.0
Using rubyzip 2.3.0
Using sassc 2.4.0
Using sassc-rails 2.1.2
Using sass-rails 6.0.0
Using selenium-webdriver 3.142.7
Using spring 2.1.1
Using spring-watcher-listen 2.0.1
Using turbolinks-source 5.2.0
Using turbolinks 5.2.1
Using web-console 4.1.0
Using webdrivers 4.5.0
Using webpacker 4.3.0
Bundle complete! 32 Gemfile dependencies, 117 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
inamurateppei@mbp iwphoto % rails s
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/pry-byebug-3.8.0/lib/pry-byebug/control_d_handler.rb:5: warning: control_d_handler's arity of 2 parameters was deprecated (eval_string, pry_instance). Now it gets passed just 1 parameter (pry_instance)
=> Booting Puma
=> Rails 6.0.3.4 application starting in development 
=> Run `rails server --help` for more startup options
warning Integrity check: Top level patterns don't match                                                                       
error Integrity check failed                                                                                                  
error Found 1 errors.                                                                                                         


========================================
  Your Yarn packages are out of date!
  Please run `yarn install --check-files` to update.
========================================


To disable this check, please change `check_yarn_integrity`
to `false` in your webpacker config file (config/webpacker.yml).


yarn check v1.22.10
info Visit https://yarnpkg.com/en/docs/cli/check for documentation about this command.


Exiting
inamurateppei@mbp iwphoto % yarn install --check-files
yarn install v1.22.10
[1/4] 🔍  Resolving packages...
[2/4] 🚚  Fetching packages...
[3/4] 🔗  Linking dependencies...
warning " > webpack-dev-server@3.11.2" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
warning "webpack-dev-server > webpack-dev-middleware@3.7.3" has unmet peer dependency "webpack@^4.0.0 || ^5.0.0".
[4/4] 🔨  Building fresh packages...
✨  Done in 154.74s.
inamurateppei@mbp iwphoto % rails s
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/pry-byebug-3.8.0/lib/pry-byebug/control_d_handler.rb:5: warning: control_d_handler's arity of 2 parameters was deprecated (eval_string, pry_instance). Now it gets passed just 1 parameter (pry_instance)
=> Booting Puma
=> Rails 6.0.3.4 application starting in development 
=> Run `rails server --help` for more startup options
Puma starting in single mode...
* Version 4.3.7 (ruby 2.6.5-p114), codename: Mysterious Traveller
* Min threads: 5, max threads: 5
* Environment: development
* Listening on tcp://127.0.0.1:3000
* Listening on tcp://[::1]:3000
Use Ctrl-C to stop
Started GET "/" for ::1 at 2021-05-22 12:40:21 +0900
   (12.2ms)  SET NAMES utf8,  @@SESSION.sql_mode = CONCAT(CONCAT(@@sql_mode, ',STRICT_ALL_TABLES'), ',NO_AUTO_VALUE_ON_ZERO'),  @@SESSION.sql_auto_is_null = 0, @@SESSION.wait_timeout = 2147483
   (3.1ms)  SELECT `schema_migrations`.`version` FROM `schema_migrations` ORDER BY `schema_migrations`.`version` ASC
  
ActiveRecord::PendingMigrationError (

Migrations are pending. To resolve this issue, run:

        rails db:migrate RAILS_ENV=development

):
  
activerecord (6.0.3.4) lib/active_record/migration.rb:586:in `check_pending!'
activerecord (6.0.3.4) lib/active_record/migration.rb:564:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/callbacks.rb:27:in `block in call'
activesupport (6.0.3.4) lib/active_support/callbacks.rb:101:in `run_callbacks'
actionpack (6.0.3.4) lib/action_dispatch/middleware/callbacks.rb:26:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/executor.rb:14:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/actionable_exceptions.rb:18:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/debug_exceptions.rb:32:in `call'
web-console (4.1.0) lib/web_console/middleware.rb:132:in `call_app'
web-console (4.1.0) lib/web_console/middleware.rb:28:in `block in call'
web-console (4.1.0) lib/web_console/middleware.rb:17:in `catch'
web-console (4.1.0) lib/web_console/middleware.rb:17:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/show_exceptions.rb:33:in `call'
railties (6.0.3.4) lib/rails/rack/logger.rb:37:in `call_app'
railties (6.0.3.4) lib/rails/rack/logger.rb:26:in `block in call'
activesupport (6.0.3.4) lib/active_support/tagged_logging.rb:80:in `block in tagged'
activesupport (6.0.3.4) lib/active_support/tagged_logging.rb:28:in `tagged'
activesupport (6.0.3.4) lib/active_support/tagged_logging.rb:80:in `tagged'
railties (6.0.3.4) lib/rails/rack/logger.rb:26:in `call'
sprockets-rails (3.2.2) lib/sprockets/rails/quiet_assets.rb:13:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/remote_ip.rb:81:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/request_id.rb:27:in `call'
rack (2.2.3) lib/rack/method_override.rb:24:in `call'
rack (2.2.3) lib/rack/runtime.rb:22:in `call'
activesupport (6.0.3.4) lib/active_support/cache/strategy/local_cache_middleware.rb:29:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/executor.rb:14:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/static.rb:126:in `call'
rack (2.2.3) lib/rack/sendfile.rb:110:in `call'
actionpack (6.0.3.4) lib/action_dispatch/middleware/host_authorization.rb:82:in `call'
webpacker (4.3.0) lib/webpacker/dev_server_proxy.rb:23:in `perform_request'
rack-proxy (0.6.5) lib/rack/proxy.rb:57:in `call'
railties (6.0.3.4) lib/rails/engine.rb:527:in `call'
puma (4.3.7) lib/puma/configuration.rb:228:in `call'
puma (4.3.7) lib/puma/server.rb:713:in `handle_request'
puma (4.3.7) lib/puma/server.rb:472:in `process_client'
puma (4.3.7) lib/puma/server.rb:328:in `block in run'
puma (4.3.7) lib/puma/thread_pool.rb:134:in `block in spawn_thread'
^C- Gracefully stopping, waiting for requests to finish
=== puma shutdown: 2021-05-22 12:40:44 +0900 ===
- Goodbye!
Exiting
inamurateppei@mbp iwphoto % rails db:migrate
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/pry-byebug-3.8.0/lib/pry-byebug/control_d_handler.rb:5: warning: control_d_handler's arity of 2 parameters was deprecated (eval_string, pry_instance). Now it gets passed just 1 parameter (pry_instance)
== 20210522014529 DeviseCreateUsers: migrating ================================
-- create_table(:users)
   -> 0.0515s
-- add_index(:users, :email, {:unique=>true})
   -> 0.0418s
-- add_index(:users, :reset_password_token, {:unique=>true})
   -> 0.0315s
== 20210522014529 DeviseCreateUsers: migrated (0.1250s) =======================

inamurateppei@mbp iwphoto % rails s  
/Users/inamurateppei/.rbenv/versions/2.6.5/lib/ruby/gems/2.6.0/gems/pry-byebug-3.8.0/lib/pry-byebug/control_d_handler.rb:5: warning: control_d_handler's arity of 2 parameters was deprecated (eval_string, pry_instance). Now it gets passed just 1 parameter (pry_instance)
=> Booting Puma
=> Rails 6.0.3.4 application starting in development 
=> Run `rails server --help` for more startup options
Puma starting in single mode...
* Version 4.3.7 (ruby 2.6.5-p114), codename: Mysterious Traveller
* Min threads: 5, max threads: 5
* Environment: development
* Listening on tcp://127.0.0.1:3000
* Listening on tcp://[::1]:3000
Use Ctrl-C to stop
Started GET "/" for ::1 at 2021-05-22 12:41:20 +0900
   (0.4ms)  SET NAMES utf8,  @@SESSION.sql_mode = CONCAT(CONCAT(@@sql_mode, ',STRICT_ALL_TABLES'), ',NO_AUTO_VALUE_ON_ZERO'),  @@SESSION.sql_auto_is_null = 0, @@SESSION.wait_timeout = 2147483
   (0.2ms)  SELECT `schema_migrations`.`version` FROM `schema_migrations` ORDER BY `schema_migrations`.`version` ASC
Processing by PhotoController#index as HTML
  Rendering photo/index.haml within layouts/application
  Rendered photo/index.haml within layouts/application (Duration: 12.3ms | Allocations: 5811)
[Webpacker] Compiling...
Started GET "/" for ::1 at 2021-05-22 12:41:24 +0900
   (0.3ms)  SET NAMES utf8,  @@SESSION.sql_mode = CONCAT(CONCAT(@@sql_mode, ',STRICT_ALL_TABLES'), ',NO_AUTO_VALUE_ON_ZERO'),  @@SESSION.sql_auto_is_null = 0, @@SESSION.wait_timeout = 2147483
Processing by PhotoController#index as HTML
  Rendering photo/index.haml within layouts/application
  Rendered photo/index.haml within layouts/application (Duration: 0.1ms | Allocations: 5)
[Webpacker] Compiling...
[Webpacker] Compiled all packs in /Users/inamurateppei/matter/iwphoto/public/packs
[Webpacker] Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.

[Webpacker] Hash: ef270c56fa66020c9089
Version: webpack 4.46.0
Time: 1600ms
Built at: 2021/05/22 12:41:24
                                     Asset       Size       Chunks                         Chunk Names
    js/application-e88c6c3304a15e6886b6.js    124 KiB  application  [emitted] [immutable]  application
js/application-e88c6c3304a15e6886b6.js.map    139 KiB  application  [emitted] [dev]        application
                             manifest.json  364 bytes               [emitted]              
Entrypoint application = js/application-e88c6c3304a15e6886b6.js js/application-e88c6c3304a15e6886b6.js.map
[./app/javascript/channels sync recursive _channel\.js$] ./app/javascript/channels sync _channel\.js$ 160 bytes {application} [built]
[./app/javascript/channels/index.js] 211 bytes {application} [built]
[./app/javascript/packs/application.js] 749 bytes {application} [built]
[./node_modules/webpack/buildin/module.js] (webpack)/buildin/module.js 552 bytes {application} [built]
    + 3 hidden modules

Completed 200 OK in 3733ms (Views: 3725.4ms | ActiveRecord: 0.0ms | Allocations: 31932)


[Webpacker] Compiled all packs in /Users/inamurateppei/matter/iwphoto/public/packs
[Webpacker] Hash: ef270c56fa66020c9089
Version: webpack 4.46.0
Time: 471ms
Built at: 2021/05/22 12:41:26
                                     Asset       Size       Chunks                         Chunk Names
    js/application-e88c6c3304a15e6886b6.js    124 KiB  application  [emitted] [immutable]  application
js/application-e88c6c3304a15e6886b6.js.map    139 KiB  application  [emitted] [dev]        application
                             manifest.json  364 bytes               [emitted]              
Entrypoint application = js/application-e88c6c3304a15e6886b6.js js/application-e88c6c3304a15e6886b6.js.map
[./app/javascript/channels sync recursive _channel\.js$] ./app/javascript/channels sync _channel\.js$ 160 bytes {application} [built]
[./app/javascript/channels/index.js] 211 bytes {application} [built]
[./app/javascript/packs/application.js] 749 bytes {application} [built]
[./node_modules/webpack/buildin/module.js] (webpack)/buildin/module.js 552 bytes {application} [built]
    + 3 hidden modules

Completed 200 OK in 1787ms (Views: 1786.8ms | ActiveRecord: 0.0ms | Allocations: 6911)


^C- Gracefully stopping, waiting for requests to finish
=== puma shutdown: 2021-05-22 12:48:19 +0900 ===
- Goodbye!
Exiting
inamurateppei@mbp iwphoto % pyenv install --list
Available versions:
  2.1.3
  2.2.3
  2.3.7
  2.4.0
  2.4.1
  2.4.2
  2.4.3
  2.4.4
  2.4.5
  2.4.6
  2.5.0
  2.5.1
  2.5.2
  2.5.3
  2.5.4
  2.5.5
  2.5.6
  2.6.6
  2.6.7
  2.6.8
  2.6.9
  2.7.0
  2.7-dev
  2.7.1
  2.7.2
  2.7.3
  2.7.4
  2.7.5
  2.7.6
  2.7.7
  2.7.8
  2.7.9
  2.7.10
  2.7.11
  2.7.12
  2.7.13
  2.7.14
  2.7.15
  2.7.16
  2.7.17
  2.7.18
  3.0.1
  3.1.0
  3.1.1
  3.1.2
  3.1.3
  3.1.4
  3.1.5
  3.2.0
  3.2.1
  3.2.2
  3.2.3
  3.2.4
  3.2.5
  3.2.6
  3.3.0
  3.3.1
  3.3.2
  3.3.3
  3.3.4
  3.3.5
  3.3.6
  3.3.7
  3.4.0
  3.4-dev
  3.4.1
  3.4.2
  3.4.3
  3.4.4
  3.4.5
  3.4.6
  3.4.7
  3.4.8
  3.4.9
  3.4.10
  3.5.0
  3.5-dev
  3.5.1
  3.5.2
  3.5.3
  3.5.4
  3.5.5
  3.5.6
  3.5.7
  3.5.8
  3.5.9
  3.5.10
  3.6.0
  3.6-dev
  3.6.1
  3.6.2
  3.6.3
  3.6.4
  3.6.5
  3.6.6
  3.6.7
  3.6.8
  3.6.9
  3.6.10
  3.6.11
  3.6.12
  3.6.13
  3.7.0
  3.7-dev
  3.7.1
  3.7.2
  3.7.3
  3.7.4
  3.7.5
  3.7.6
  3.7.7
  3.7.8
  3.7.9
  3.7.10
  3.8.0
  3.8-dev
  3.8.1
  3.8.2
  3.8.3
  3.8.4
  3.8.5
  3.8.6
  3.8.7
  3.8.8
  3.8.9
  3.9.0
  3.9-dev
  3.9.1
  3.9.2
  3.9.3
  3.9.4
  3.10.0a7
  3.10-dev
  activepython-2.7.14
  activepython-3.5.4
  activepython-3.6.0
  anaconda-1.4.0
  anaconda-1.5.0
  anaconda-1.5.1
  anaconda-1.6.0
  anaconda-1.6.1
  anaconda-1.7.0
  anaconda-1.8.0
  anaconda-1.9.0
  anaconda-1.9.1
  anaconda-1.9.2
  anaconda-2.0.0
  anaconda-2.0.1
  anaconda-2.1.0
  anaconda-2.2.0
  anaconda-2.3.0
  anaconda-2.4.0
  anaconda-4.0.0
  anaconda2-2.4.0
  anaconda2-2.4.1
  anaconda2-2.5.0
  anaconda2-4.0.0
  anaconda2-4.1.0
  anaconda2-4.1.1
  anaconda2-4.2.0
  anaconda2-4.3.0
  anaconda2-4.3.1
  anaconda2-4.4.0
  anaconda2-5.0.0
  anaconda2-5.0.1
  anaconda2-5.1.0
  anaconda2-5.2.0
  anaconda2-5.3.0
  anaconda2-5.3.1
  anaconda2-2018.12
  anaconda2-2019.03
  anaconda2-2019.07
  anaconda3-2.0.0
  anaconda3-2.0.1
  anaconda3-2.1.0
  anaconda3-2.2.0
  anaconda3-2.3.0
  anaconda3-2.4.0
  anaconda3-2.4.1
  anaconda3-2.5.0
  anaconda3-4.0.0
  anaconda3-4.1.0
  anaconda3-4.1.1
  anaconda3-4.2.0
  anaconda3-4.3.0
  anaconda3-4.3.1
  anaconda3-4.4.0
  anaconda3-5.0.0
  anaconda3-5.0.1
  anaconda3-5.1.0
  anaconda3-5.2.0
  anaconda3-5.3.0
  anaconda3-5.3.1
  anaconda3-2018.12
  anaconda3-2019.03
  anaconda3-2019.07
  anaconda3-2019.10
  anaconda3-2020.02
  anaconda3-2020.07
  anaconda3-2020.11
  graalpython-20.1.0
  graalpython-20.2.0
  graalpython-20.3.0
  graalpython-21.0.0
  graalpython-21.1.0
  ironpython-dev
  ironpython-2.7.4
  ironpython-2.7.5
  ironpython-2.7.6.3
  ironpython-2.7.7
  jython-dev
  jython-2.5.0
  jython-2.5-dev
  jython-2.5.1
  jython-2.5.2
  jython-2.5.3
  jython-2.5.4-rc1
  jython-2.7.0
  jython-2.7.1
  jython-2.7.2
  micropython-dev
  micropython-1.9.3
  micropython-1.9.4
  micropython-1.10
  micropython-1.11
  micropython-1.12
  micropython-1.13
  micropython-1.14
  miniconda-latest
  miniconda-2.2.2
  miniconda-3.0.0
  miniconda-3.0.4
  miniconda-3.0.5
  miniconda-3.3.0
  miniconda-3.4.2
  miniconda-3.7.0
  miniconda-3.8.3
  miniconda-3.9.1
  miniconda-3.10.1
  miniconda-3.16.0
  miniconda-3.18.3
  miniconda2-latest
  miniconda2-3.18.3
  miniconda2-3.19.0
  miniconda2-4.0.5
  miniconda2-4.1.11
  miniconda2-4.3.14
  miniconda2-4.3.21
  miniconda2-4.3.27
  miniconda2-4.3.30
  miniconda2-4.3.31
  miniconda2-4.4.10
  miniconda2-4.5.1
  miniconda2-4.5.4
  miniconda2-4.5.11
  miniconda2-4.5.12
  miniconda2-4.6.14
  miniconda2-4.7.10
  miniconda2-4.7.12
  miniconda3-latest
  miniconda3-2.2.2
  miniconda3-3.0.0
  miniconda3-3.0.4
  miniconda3-3.0.5
  miniconda3-3.3.0
  miniconda3-3.4.2
  miniconda3-3.7.0
  miniconda3-3.7-4.8.2
  miniconda3-3.7-4.8.3
  miniconda3-3.7-4.9.2
  miniconda3-3.8.3
  miniconda3-3.8-4.8.2
  miniconda3-3.8-4.8.3
  miniconda3-3.8-4.9.2
  miniconda3-3.9.1
  miniconda3-3.9-4.9.2
  miniconda3-3.10.1
  miniconda3-3.16.0
  miniconda3-3.18.3
  miniconda3-3.19.0
  miniconda3-4.0.5
  miniconda3-4.1.11
  miniconda3-4.2.12
  miniconda3-4.3.11
  miniconda3-4.3.14
  miniconda3-4.3.21
  miniconda3-4.3.27
  miniconda3-4.3.30
  miniconda3-4.3.31
  miniconda3-4.4.10
  miniconda3-4.5.1
  miniconda3-4.5.4
  miniconda3-4.5.11
  miniconda3-4.5.12
  miniconda3-4.6.14
  miniconda3-4.7.10
  miniconda3-4.7.12
  miniforge3-4.9.2
  miniforge3-4.10
  pypy-c-jit-latest
  pypy-dev
  pypy-stm-2.3
  pypy-stm-2.5.1
  pypy-1.5-src
  pypy-1.6
  pypy-1.7
  pypy-1.8
  pypy-1.9
  pypy-2.0-src
  pypy-2.0
  pypy-2.0.1-src
  pypy-2.0.1
  pypy-2.0.2-src
  pypy-2.0.2
  pypy-2.1-src
  pypy-2.1
  pypy-2.2-src
  pypy-2.2
  pypy-2.2.1-src
  pypy-2.2.1
  pypy-2.3-src
  pypy-2.3
  pypy-2.3.1-src
  pypy-2.3.1
  pypy-2.4.0-src
  pypy-2.4.0
  pypy-2.5.0-src
  pypy-2.5.0
  pypy-2.5.1-src
  pypy-2.5.1
  pypy-2.6.0-src
  pypy-2.6.0
  pypy-2.6.1-src
  pypy-2.6.1
  pypy-4.0.0-src
  pypy-4.0.0
  pypy-4.0.1-src
  pypy-4.0.1
  pypy-5.0.0-src
  pypy-5.0.0
  pypy-5.0.1-src
  pypy-5.0.1
  pypy-5.1-src
  pypy-5.1
  pypy-5.1.1-src
  pypy-5.1.1
  pypy-5.3-src
  pypy-5.3
  pypy-5.3.1-src
  pypy-5.3.1
  pypy-5.4-src
  pypy-5.4
  pypy-5.4.1-src
  pypy-5.4.1
  pypy-5.6.0-src
  pypy-5.6.0
  pypy-5.7.0-src
  pypy-5.7.0
  pypy-5.7.1-src
  pypy-5.7.1
  pypy2-5.3-src
  pypy2-5.3
  pypy2-5.3.1-src
  pypy2-5.3.1
  pypy2-5.4-src
  pypy2-5.4
  pypy2-5.4.1-src
  pypy2-5.4.1
  pypy2-5.6.0-src
  pypy2-5.6.0
  pypy2-5.7.0-src
  pypy2-5.7.0
  pypy2-5.7.1-src
  pypy2-5.7.1
  pypy2.7-5.8.0-src
  pypy2.7-5.8.0
  pypy2.7-5.9.0-src
  pypy2.7-5.9.0
  pypy2.7-5.10.0-src
  pypy2.7-5.10.0
  pypy2.7-6.0.0-src
  pypy2.7-6.0.0
  pypy2.7-7.0.0-src
  pypy2.7-7.0.0
  pypy2.7-7.1.0-src
  pypy2.7-7.1.0
  pypy2.7-7.1.1-src
  pypy2.7-7.1.1
  pypy2.7-7.2.0-src
  pypy2.7-7.2.0
  pypy2.7-7.3.0-src
  pypy2.7-7.3.0
  pypy2.7-7.3.1-src
  pypy2.7-7.3.1
  pypy3-2.3.1-src
  pypy3-2.3.1
  pypy3-2.4.0-src
  pypy3-2.4.0
  pypy3.3-5.2-alpha1-src
  pypy3.3-5.2-alpha1
  pypy3.3-5.5-alpha-src
  pypy3.3-5.5-alpha
  pypy3.5-c-jit-latest
  pypy3.5-5.7-beta-src
  pypy3.5-5.7-beta
  pypy3.5-5.7.1-beta-src
  pypy3.5-5.7.1-beta
  pypy3.5-5.8.0-src
  pypy3.5-5.8.0
  pypy3.5-5.9.0-src
  pypy3.5-5.9.0
  pypy3.5-5.10.0-src
  pypy3.5-5.10.0
  pypy3.5-5.10.1-src
  pypy3.5-5.10.1
  pypy3.5-6.0.0-src
  pypy3.5-6.0.0
  pypy3.5-7.0.0-src
  pypy3.5-7.0.0
  pypy3.6-7.0.0-src
  pypy3.6-7.0.0
  pypy3.6-7.1.0-src
  pypy3.6-7.1.0
  pypy3.6-7.1.1-src
  pypy3.6-7.1.1
  pypy3.6-7.2.0-src
  pypy3.6-7.2.0
  pypy3.6-7.3.0-src
  pypy3.6-7.3.0
  pypy3.6-7.3.1-src
  pypy3.6-7.3.1
  pypy3.6-7.3.2-src
  pypy3.6-7.3.2
  pypy3.6-7.3.3-src
  pypy3.6-7.3.3
  pypy3.7-c-jit-latest
  pypy3.7-7.3.2-src
  pypy3.7-7.3.2
  pypy3.7-7.3.3-src
  pypy3.7-7.3.3
  pypy3.7-7.3.4
  pyston-0.5.1
  pyston-0.6.0
  pyston-0.6.1
  stackless-dev
  stackless-2.7-dev
  stackless-2.7.2
  stackless-2.7.3
  stackless-2.7.4
  stackless-2.7.5
  stackless-2.7.6
  stackless-2.7.7
  stackless-2.7.8
  stackless-2.7.9
  stackless-2.7.10
  stackless-2.7.11
  stackless-2.7.12
  stackless-2.7.14
  stackless-3.2.2
  stackless-3.2.5
  stackless-3.3.5
  stackless-3.3.7
  stackless-3.4-dev
  stackless-3.4.2
  stackless-3.4.7
  stackless-3.5.4
  stackless-3.7.5
inamurateppei@mbp iwphoto % pyenv install 3.6.5
python-build: use openssl from homebrew
python-build: use readline from homebrew
Downloading Python-3.6.5.tar.xz...
-> https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tar.xz
Installing Python-3.6.5...
python-build: use readline from homebrew
python-build: use zlib from xcode sdk

BUILD FAILED (OS X 11.2.3 using python-build 20180424)

Inspect or clean up the working tree at /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522125118.39758
Results logged to /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522125118.39758.log

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
inamurateppei@mbp iwphoto % ls
Gemfile			app			config.ru		log			public			tmp
Gemfile.lock		babel.config.js		db			node_modules		spec			vendor
README.md		bin			er.dio			package.json		storage			yarn.lock
Rakefile		config			lib			postcss.config.js	test
inamurateppei@mbp iwphoto % cd
inamurateppei@mbp ~ % pyenv -v
pyenv 1.2.27
inamurateppei@mbp ~ % echo $SHELL
/bin/zsh
inamurateppei@mbp ~ % echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
inamurateppei@mbp ~ % echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
inamurateppei@mbp ~ % echo 'eval "$(pyenv init -)"' >> ~/.zshrc
inamurateppei@mbp ~ % source ~/.zshrc
inamurateppei@mbp ~ % pyenv install 3.6.5
python-build: use openssl from homebrew
python-build: use readline from homebrew
Downloading Python-3.6.5.tar.xz...
-> https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tar.xz
Installing Python-3.6.5...
python-build: use readline from homebrew
python-build: use zlib from xcode sdk

BUILD FAILED (OS X 11.2.3 using python-build 20180424)

Inspect or clean up the working tree at /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522125455.50591
Results logged to /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210522125455.50591.log

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
inamurateppei@mbp ~ % LDFLAGS="-L$(xcrun --show-sdk-path)/usr/lib" pyenv install 3.6.5
python-build: use openssl from homebrew
python-build: use readline from homebrew
Downloading Python-3.6.5.tar.xz...
-> https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tar.xz
Installing Python-3.6.5...
python-build: use readline from homebrew
python-build: use zlib from xcode sdk

BUILD FAILED (OS X 11.2.3 using python-build 20180424)

Inspect or clean up the working tree at /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210523092222.67719
Results logged to /var/folders/3z/nrjs__rs3gl5l6_3qtkyt8240000gn/T/python-build.20210523092222.67719.log

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
inamurateppei@mbp ~ % brew update
Updated 2 taps (homebrew/core and homebrew/services).
==> New Formulae
proj@7
==> Updated Formulae
armadillo            exploitdb            libgeotiff           mysql++              sngrep
autorest             fluent-bit           librasterlite        mysql-connector-c++  snowpack
autorestic           fonttools            libsass              name-that-hash       spatialite-gui
aws-sdk-cpp          freeipmi             libspatialite        netlify-cli          spatialite-tools
b2-tools             fzf                  libunwind-headers    nift                 sphinx-doc
bettercap            gdal                 logrotate            node-sass            ssh-vault
byacc                gdu                  mapnik               ocrmypdf             swiftformat
cairomm              geoserver            mapserver            open-zwave           synfig
cargo-instruments    ghq                  marked               osm2pgsql            texlab
cdogs-sdl            gradle               matplotplusplus      pandoc-plot          tfsec
chart-testing        gradle@6             mesa                 pgpool-ii            timelimit
ckan                 gtkmm3               mingw-w64            postgis              todoman
cmusfm               gtkmm4               minio                pre-commit           trash-cli
comby                halide               mkvtoolnix           proj                 truffle
daemon               ipv6calc             mlt                  richmd               twarc
darcs                libepoxy             moto                 simdjson             watchexec
eslint               libgaiagraphics      mpd                  snakemake            yq

You have 38 outdated formulae installed.
You can upgrade them with brew upgrade
or list them with brew outdated.
inamurateppei@mbp ~ % brew upgrade
==> Upgrading 38 outdated packages:
libheif 1.11.0 -> 1.12.0
terraform 0.14.3 -> 0.15.4
libtiff 4.2.0 -> 4.3.0
libtool 2.4.6_2 -> 2.4.6_3
xorgproto 2021.3 -> 2021.4
ilmbase 2.5.5 -> 2.5.5_1
ghostscript 9.53.3_1 -> 9.54.0
heroku/brew/heroku 7.46.2 -> 7.54.0
gdbm 1.18.1_1 -> 1.19
pango 1.48.2 -> 1.48.5
gdk-pixbuf 2.42.2 -> 2.42.6
icu4c 68.2 -> 69.1
harfbuzz 2.7.4_1 -> 2.8.1
glib 2.66.7 -> 2.68.2
netpbm 10.86.18 -> 10.86.22
aom 2.0.2 -> 3.1.0
awscli 2.1.13 -> 2.2.5
sqlite 3.34.0 -> 3.35.5
gobject-introspection 1.66.1_1 -> 1.68.0
openexr 2.5.5 -> 3.0.3
librsvg 2.50.3 -> 2.50.5
mysql 8.0.23_1 -> 8.0.25_1
graphviz 2.46.1 -> 2.47.1
heroku/brew/heroku-node 12.16.2 -> 12.21.0
gd 2.3.1 -> 2.3.2
tfenv 2.0.0 -> 2.2.2
x265 3.4_2 -> 3.5
node 15.5.1 -> 16.2.0
libomp 11.1.0 -> 12.0.0
python@3.8 3.8.6_2 -> 3.8.10
imagemagick 7.0.11-2 -> 7.0.11-13_2
jasper 2.0.25 -> 2.0.32
libx11 1.7.0 -> 1.7.1
protobuf 3.15.8 -> 3.17.0_1
git 2.30.1 -> 2.31.1
amazon-ecs-cli 1.20.0 -> 1.21.0
libffi 3.3_2 -> 3.3_3
python@3.9 3.9.2_1 -> 3.9.5
==> Upgrading heroku/brew/heroku-node 12.16.2 -> 12.21.0 
==> Downloading https://nodejs.org/download/release/v12.21.0/node-v12.21.0-darwin-x64.tar.xz
######################################################################## 100.0%
Error: The `brew link` step did not complete successfully
The formula built, but is not symlinked into /usr/local
Could not symlink bin/node
Target /usr/local/bin/node
already exists. You may want to remove it:
  rm '/usr/local/bin/node'

To force the link and overwrite all conflicting files:
  brew link --overwrite heroku-node

To list all files that would be deleted:
  brew link --overwrite --dry-run heroku-node

Possible conflicting files are:
/usr/local/bin/node
==> Caveats
heroku-node is keg-only, which means it was not symlinked into /usr/local,
because heroku-node is only used by Heroku CLI (heroku/brew/heroku), which explicitly requires from Cellar.

If you need to have heroku-node first in your PATH, run:
  echo 'export PATH="/usr/local/opt/heroku-node/bin:$PATH"' >> ~/.zshrc

==> Summary
🍺  /usr/local/Cellar/heroku-node/12.21.0: 6 files, 45.4MB, built in 11 seconds
Removing: /usr/local/Cellar/heroku-node/12.16.2... (3 files, 42.2MB)
==> Upgrading sqlite 3.34.0 -> 3.35.5 
==> Downloading https://ghcr.io/v2/homebrew/core/sqlite/manifests/3.35.5
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/378ec4b4eabacb2e78491282aed532b43a440467b1b9de74c128b026d3c912ba--sqlite-3.35.5.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/sqlite/blobs/sha256:801e11dff40b2e7067b8e124d266f82050cbae
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/1a664fe49a26a15104a30b571869e6eb8d8f841848f89795ffa95939f82c3055--sqlite--3.35.5.big_sur.bottle.tar.gz
==> Pouring sqlite--3.35.5.big_sur.bottle.tar.gz
==> Caveats
sqlite is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have sqlite first in your PATH, run:
  echo 'export PATH="/usr/local/opt/sqlite/bin:$PATH"' >> ~/.zshrc

For compilers to find sqlite you may need to set:
  export LDFLAGS="-L/usr/local/opt/sqlite/lib"
  export CPPFLAGS="-I/usr/local/opt/sqlite/include"

For pkg-config to find sqlite you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/sqlite/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/sqlite/3.35.5: 11 files, 4.2MB
Removing: /usr/local/Cellar/sqlite/3.34.0... (11 files, 4.1MB)
==> Upgrading python@3.8 3.8.6_2 -> 3.8.10 
==> Downloading https://ghcr.io/v2/homebrew/core/gdbm/manifests/1.19
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/bf3024395228e8948861d356d9effabe26c0194b4b55f2dc07a67bd38c834381--gdbm-1.19.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/gdbm/blobs/sha256:3581501b051db1c0d1acccc710fe04453b61777e
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/19b0b9d79e157a2af6620cdb9846df478b61f213837dbae6763c32195614be73--gdbm--1.19.big_sur.bottle.tar.gz
==> Downloading https://ghcr.io/v2/homebrew/core/python/3.8/manifests/3.8.10
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/python/3.8/blobs/sha256:52b3504c2c9e63ded764f97352194fd49f
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:52b3504c2c9e63ded764f9
######################################################################## 100.0%
==> Installing dependencies for python@3.8: gdbm
==> Installing python@3.8 dependency: gdbm
==> Pouring gdbm--1.19.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/gdbm/1.19: 24 files, 791.3KB
==> Installing python@3.8
==> Pouring python@3.8--3.8.10.big_sur.bottle.tar.gz
==> /usr/local/Cellar/python@3.8/3.8.10/bin/python3 -s setup.py --no-user-cfg install --force --verbose --i
==> /usr/local/Cellar/python@3.8/3.8.10/bin/python3 -s setup.py --no-user-cfg install --force --verbose --i
==> /usr/local/Cellar/python@3.8/3.8.10/bin/python3 -s setup.py --no-user-cfg install --force --verbose --i
==> Caveats
Python has been installed as
  /usr/local/opt/python@3.8/bin/python3

Unversioned symlinks `python`, `python-config`, `pip` etc. pointing to
`python3`, `python3-config`, `pip3` etc., respectively, have been installed into
  /usr/local/opt/python@3.8/libexec/bin

You can install Python packages with
  /usr/local/opt/python@3.8/bin/pip3 install <package>
They will install into the site-package directory
  /usr/local/lib/python3.8/site-packages

See: https://docs.brew.sh/Homebrew-and-Python

python@3.8 is keg-only, which means it was not symlinked into /usr/local,
because this is an alternate version of another formula.

If you need to have python@3.8 first in your PATH, run:
  echo 'export PATH="/usr/local/opt/python@3.8/bin:$PATH"' >> ~/.zshrc

For compilers to find python@3.8 you may need to set:
  export LDFLAGS="-L/usr/local/opt/python@3.8/lib"

For pkg-config to find python@3.8 you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/python@3.8/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/python@3.8/3.8.10: 4,423 files, 71.2MB
Removing: /usr/local/Cellar/python@3.8/3.8.6_2... (4,329 files, 69.4MB)
==> Upgrading icu4c 68.2 -> 69.1 
==> Downloading https://ghcr.io/v2/homebrew/core/icu4c/manifests/69.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/icu4c/blobs/sha256:d46b8ec5c3db629e7848e9fd31e5ec99ed952d9
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:d46b8ec5c3db629e7848e9
######################################################################## 100.0%
==> Pouring icu4c--69.1.big_sur.bottle.tar.gz
==> Caveats
icu4c is keg-only, which means it was not symlinked into /usr/local,
because macOS provides libicucore.dylib (but nothing else).

If you need to have icu4c first in your PATH, run:
  echo 'export PATH="/usr/local/opt/icu4c/bin:$PATH"' >> ~/.zshrc
  echo 'export PATH="/usr/local/opt/icu4c/sbin:$PATH"' >> ~/.zshrc

For compilers to find icu4c you may need to set:
  export LDFLAGS="-L/usr/local/opt/icu4c/lib"
  export CPPFLAGS="-I/usr/local/opt/icu4c/include"

For pkg-config to find icu4c you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/icu4c/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/icu4c/69.1: 259 files, 72.8MB
Removing: /usr/local/Cellar/icu4c/68.2... (259 files, 72.5MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/icu4c--68.2.big_sur.bottle.tar.gz... (27.1MB)
==> Upgrading libffi 3.3_2 -> 3.3_3 
==> Downloading https://ghcr.io/v2/homebrew/core/libffi/manifests/3.3_3
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/579ebe43f9cb570f21b0b4deb5906e9e833291b57639d94ff691b9377cbfdddd--libffi-3.3_3.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/libffi/blobs/sha256:8a7a02cffb368dfdeaeb1176a7a7bcc6402371
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/8f0286cf28930b83052c9ddff88bd4cc4636bbde4b0c78e67bcbcfa794337937--libffi--3.3_3.big_sur.bottle.tar.gz
==> Pouring libffi--3.3_3.big_sur.bottle.tar.gz
==> Caveats
libffi is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

For compilers to find libffi you may need to set:
  export LDFLAGS="-L/usr/local/opt/libffi/lib"
  export CPPFLAGS="-I/usr/local/opt/libffi/include"

For pkg-config to find libffi you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/libffi/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/libffi/3.3_3: 17 files, 540.5KB
Removing: /usr/local/Cellar/libffi/3.3_2... (17 files, 540.5KB)
==> Upgrading ilmbase 2.5.5 -> 2.5.5_1 
Warning: ilmbase has been deprecated because it is not supported upstream!
==> Downloading https://ghcr.io/v2/homebrew/core/ilmbase/manifests/2.5.5_1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ilmbase/blobs/sha256:846c944f66f265e002af5f3ba3f2a989fbbc8
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:846c944f66f265e002af5f
######################################################################## 100.0%
==> Pouring ilmbase--2.5.5_1.big_sur.bottle.tar.gz
==> Caveats
`ilmbase` has been replaced by `imath`. You may want to `brew uninstall ilmbase`
or `brew unlink ilmbase` to prevent conflicts.

ilmbase is keg-only, which means it was not symlinked into /usr/local,
because ilmbase conflicts with `openexr` and `imath`.

For compilers to find ilmbase you may need to set:
  export LDFLAGS="-L/usr/local/opt/ilmbase/lib"
  export CPPFLAGS="-I/usr/local/opt/ilmbase/include"

For pkg-config to find ilmbase you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/ilmbase/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/ilmbase/2.5.5_1: 87 files, 1.8MB
Removing: /usr/local/Cellar/ilmbase/2.5.5... (87 files, 1.8MB)
==> Upgrading heroku/brew/heroku 7.46.2 -> 7.54.0 
==> Downloading https://cli-assets.heroku.com/heroku-v7.54.0/heroku-v7.54.0.tar.xz
######################################################################## 100.0%
==> Caveats
To use the Heroku CLI's autocomplete --
  Via homebrew's shell completion:
    1) Follow homebrew's install instructions https://docs.brew.sh/Shell-Completion
        NOTE: For zsh, as the instructions mention, be sure compinit is autoloaded
              and called, either explicitly or via a framework like oh-my-zsh.
    2) Then run
      $ heroku autocomplete --refresh-cache
  OR
  Use our standalone setup:
    1) Run and follow the install steps:
      $ heroku autocomplete

zsh completions have been installed to:
  /usr/local/share/zsh/site-functions
==> Summary
🍺  /usr/local/Cellar/heroku/7.54.0: 28,788 files, 62.9MB, built in 48 seconds
Removing: /usr/local/Cellar/heroku/7.46.2... (82,416 files, 262.8MB)
==> Upgrading gdbm 1.19 -> 1.19 
Removing: /usr/local/Cellar/gdbm/1.18.1_1... (25 files, 641KB)
==> Upgrading pango 1.48.2 -> 1.48.5 
==> Downloading https://ghcr.io/v2/homebrew/core/python/3.9/manifests/3.9.5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/python/3.9/blobs/sha256:316baac980aa0a3dac263d64de41c4f09b
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:316baac980aa0a3dac263d
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/glib/manifests/2.68.2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/glib/blobs/sha256:e33dfc5c9d1db7709398d6e5eaa7c3606398261f
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:e33dfc5c9d1db7709398d6
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/xorgproto/manifests/2021.4
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/xorgproto/blobs/sha256:e7e892aa9dfd101f067d5c3e298ccc65bb3
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:e7e892aa9dfd101f067d5c
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libx11/manifests/1.7.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libx11/blobs/sha256:9998bb9f54cc7ee1c11cc5dd645efa2ab07542
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:9998bb9f54cc7ee1c11cc5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gobject-introspection/manifests/1.68.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gobject-introspection/blobs/sha256:bea661944345fe41b302c36
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:bea661944345fe41b302c3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/harfbuzz/manifests/2.8.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/harfbuzz/blobs/sha256:c058750b71d64974110c4fdf3dac4cb4ccd3
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:c058750b71d64974110c4f
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pango/manifests/1.48.5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pango/blobs/sha256:cabbacd4559bb2c843f6e4965f65c6baf5e66a5
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:cabbacd4559bb2c843f6e4
######################################################################## 100.0%
==> Installing dependencies for pango: python@3.9, glib, xorgproto, libx11, gobject-introspection and harfbuzz
==> Installing pango dependency: python@3.9
==> Pouring python@3.9--3.9.5.big_sur.bottle.tar.gz
==> /usr/local/Cellar/python@3.9/3.9.5/bin/python3 -m ensurepip
==> /usr/local/Cellar/python@3.9/3.9.5/bin/python3 -m pip install -v --no-deps --no-index --upgrade --isola
==> Caveats
Python has been installed as
  /usr/local/bin/python3

Unversioned symlinks `python`, `python-config`, `pip` etc. pointing to
`python3`, `python3-config`, `pip3` etc., respectively, have been installed into
  /usr/local/opt/python@3.9/libexec/bin

You can install Python packages with
  pip3 install <package>
They will install into the site-package directory
  /usr/local/lib/python3.9/site-packages

tkinter is no longer included with this formula, but it is available separately:
  brew install python-tk@3.9

See: https://docs.brew.sh/Homebrew-and-Python
==> Summary
🍺  /usr/local/Cellar/python@3.9/3.9.5: 3,078 files, 54.5MB
==> Installing pango dependency: glib
==> Pouring glib--2.68.2.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/glib/2.68.2: 442 files, 21MB
==> Installing pango dependency: xorgproto
==> Pouring xorgproto--2021.4.all.bottle.tar.gz
🍺  /usr/local/Cellar/xorgproto/2021.4: 264 files, 3.9MB
==> Installing pango dependency: libx11
==> Pouring libx11--1.7.1.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/libx11/1.7.1: 1,055 files, 7MB
==> Installing pango dependency: gobject-introspection
==> Pouring gobject-introspection--1.68.0.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/gobject-introspection/1.68.0: 190 files, 12.7MB
==> Installing pango dependency: harfbuzz
==> Pouring harfbuzz--2.8.1.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/harfbuzz/2.8.1: 68 files, 7MB
==> Installing pango
==> Pouring pango--1.48.5.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/pango/1.48.5: 64 files, 2.9MB
Removing: /usr/local/Cellar/pango/1.48.2... (64 files, 3MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/pango--1.48.2.big_sur.bottle.tar.gz... (734.7KB)
==> Upgrading gdk-pixbuf 2.42.2 -> 2.42.6 
==> Downloading https://ghcr.io/v2/homebrew/core/libtiff/manifests/4.3.0
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/c24b87e3eea7ffd536298b1b0782aa3506514ec9547e00fd90cde106f050376a--libtiff-4.3.0.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/libtiff/blobs/sha256:09f08e1168780c12c8f1526038eb4f4692624
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/54a8d701eebf8cb3e7c581e9ad168ed4cc077ec43419b50a2052be92eb13bb27--libtiff--4.3.0.big_sur.bottle.tar.gz
==> Downloading https://ghcr.io/v2/homebrew/core/gdk-pixbuf/manifests/2.42.6
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gdk-pixbuf/blobs/sha256:f4cf795b20c84fb5074ceeeeaf7b1d22e1
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:f4cf795b20c84fb5074cee
######################################################################## 100.0%
==> Installing dependencies for gdk-pixbuf: libtiff
==> Installing gdk-pixbuf dependency: libtiff
==> Pouring libtiff--4.3.0.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/libtiff/4.3.0: 249 files, 4.4MB
==> Installing gdk-pixbuf
==> Pouring gdk-pixbuf--2.42.6.big_sur.bottle.tar.gz
==> /usr/local/Cellar/gdk-pixbuf/2.42.6/bin/gdk-pixbuf-query-loaders --update-cache
🍺  /usr/local/Cellar/gdk-pixbuf/2.42.6: 147 files, 3.7MB
Removing: /usr/local/Cellar/gdk-pixbuf/2.42.2... (149 files, 3.8MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/gdk-pixbuf--2.42.2.big_sur.bottle.tar.gz... (801.3KB)
==> Upgrading harfbuzz 2.8.1 -> 2.8.1 
Removing: /usr/local/Cellar/harfbuzz/2.7.4_1... (68 files, 6.7MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/harfbuzz--2.7.4_1.big_sur.bottle.tar.gz... (2.0MB)
==> Upgrading glib 2.68.2 -> 2.68.2 
Removing: /usr/local/Cellar/glib/2.66.7... (441 files, 20.8MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/glib--2.66.7.big_sur.bottle.tar.gz... (6.2MB)
==> Upgrading netpbm 10.86.18 -> 10.86.22 
==> Downloading https://ghcr.io/v2/homebrew/core/jasper/manifests/2.0.32
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/jasper/blobs/sha256:3b56f3d1d584df4483b5d35d5d75235bd62120
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:3b56f3d1d584df4483b5d3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/netpbm/manifests/10.86.22
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/netpbm/blobs/sha256:e2254237db71e5278c239560583a9de64c94f6
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:e2254237db71e5278c2395
######################################################################## 100.0%
==> Installing dependencies for netpbm: jasper
==> Installing netpbm dependency: jasper
==> Pouring jasper--2.0.32.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/jasper/2.0.32: 40 files, 1018.8KB
==> Installing netpbm
==> Pouring netpbm--10.86.22.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/netpbm/10.86.22: 410 files, 17.8MB
Removing: /usr/local/Cellar/netpbm/10.86.18... (410 files, 17.7MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/netpbm--10.86.18.big_sur.bottle.tar.gz... (1.8MB)
==> Upgrading aom 2.0.2 -> 3.1.0 
==> Downloading https://ghcr.io/v2/homebrew/core/aom/manifests/3.1.0
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/4330797f41cf1f4089b82c134b718a48800b5e3d433eefce830a688fee9b1e02--aom-3.1.0.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/aom/blobs/sha256:b01451365abb2da2a9b17d2aff9fba994e90b3718
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/abc0abc96633bd2f19fdb28fd2f00ef5eb3df4e653e91052818fe4821dd3ae45--aom--3.1.0.big_sur.bottle.tar.gz
==> Pouring aom--3.1.0.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/aom/3.1.0: 22 files, 12.6MB
Removing: /usr/local/Cellar/aom/2.0.2... (22 files, 11.5MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/aom--2.0.2.big_sur.bottle.tar.gz... (3.9MB)
==> Upgrading awscli 2.1.13 -> 2.2.5 
==> Downloading https://ghcr.io/v2/homebrew/core/awscli/manifests/2.2.5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/awscli/blobs/sha256:a7d80cf7dd99d2c3ffa15f512898d8a3c9b315
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:a7d80cf7dd99d2c3ffa15f
######################################################################## 100.0%
==> Pouring awscli--2.2.5.big_sur.bottle.tar.gz
==> Caveats
The "examples" directory has been installed to:
  /usr/local/share/awscli/examples

zsh completions and functions have been installed to:
  /usr/local/share/zsh/site-functions
==> Summary
🍺  /usr/local/Cellar/awscli/2.2.5: 12,706 files, 100.3MB
Removing: /usr/local/Cellar/awscli/2.1.13... (12,524 files, 94.8MB)
==> Upgrading gobject-introspection 1.68.0 -> 1.68.0 
Removing: /usr/local/Cellar/gobject-introspection/1.66.1_1... (191 files, 12.7MB)
==> Upgrading openexr 2.5.5 -> 3.0.3 
==> Downloading https://ghcr.io/v2/homebrew/core/imath/manifests/3.0.3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/imath/blobs/sha256:c8ff0ac963b448ef81fd594fd34ac58786240e0
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:c8ff0ac963b448ef81fd59
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openexr/manifests/3.0.3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openexr/blobs/sha256:0df22b8bfaeecf3be5d8e87f79fff487e2017
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:0df22b8bfaeecf3be5d8e8
######################################################################## 100.0%
==> Installing dependencies for openexr: imath
==> Installing openexr dependency: imath
==> Pouring imath--3.0.3.big_sur.bottle.tar.gz
Error: The `brew link` step did not complete successfully
The formula built, but is not symlinked into /usr/local
Could not symlink lib/libImath.dylib
Target /usr/local/lib/libImath.dylib
is a symlink belonging to ilmbase. You can unlink it:
  brew unlink ilmbase

To force the link and overwrite all conflicting files:
  brew link --overwrite imath

To list all files that would be deleted:
  brew link --overwrite --dry-run imath

Possible conflicting files are:
/usr/local/lib/libImath.dylib -> /usr/local/Cellar/ilmbase/2.5.5_1/lib/libImath.dylib
==> Summary
🍺  /usr/local/Cellar/imath/3.0.3: 49 files, 885.8KB
==> Installing openexr
==> Pouring openexr--3.0.3.big_sur.bottle.tar.gz
Error: The `brew link` step did not complete successfully
The formula built, but is not symlinked into /usr/local
Could not symlink include/OpenEXR/Iex.h
Target /usr/local/include/OpenEXR/Iex.h
is a symlink belonging to ilmbase. You can unlink it:
  brew unlink ilmbase

To force the link and overwrite all conflicting files:
  brew link --overwrite openexr

To list all files that would be deleted:
  brew link --overwrite --dry-run openexr

Possible conflicting files are:
/usr/local/include/OpenEXR/Iex.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/Iex.h
/usr/local/include/OpenEXR/IexBaseExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexBaseExc.h
/usr/local/include/OpenEXR/IexErrnoExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexErrnoExc.h
/usr/local/include/OpenEXR/IexExport.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexExport.h
/usr/local/include/OpenEXR/IexForward.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexForward.h
/usr/local/include/OpenEXR/IexMacros.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexMacros.h
/usr/local/include/OpenEXR/IexMathExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexMathExc.h
/usr/local/include/OpenEXR/IexMathFloatExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexMathFloatExc.h
/usr/local/include/OpenEXR/IexMathIeeeExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexMathIeeeExc.h
/usr/local/include/OpenEXR/IexNamespace.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexNamespace.h
/usr/local/include/OpenEXR/IexThrowErrnoExc.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IexThrowErrnoExc.h
/usr/local/include/OpenEXR/IlmThread.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThread.h
/usr/local/include/OpenEXR/IlmThreadExport.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadExport.h
/usr/local/include/OpenEXR/IlmThreadForward.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadForward.h
/usr/local/include/OpenEXR/IlmThreadMutex.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadMutex.h
/usr/local/include/OpenEXR/IlmThreadNamespace.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadNamespace.h
/usr/local/include/OpenEXR/IlmThreadPool.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadPool.h
/usr/local/include/OpenEXR/IlmThreadSemaphore.h -> /usr/local/Cellar/ilmbase/2.5.5_1/include/OpenEXR/IlmThreadSemaphore.h
/usr/local/lib/libIex.dylib -> /usr/local/Cellar/ilmbase/2.5.5_1/lib/libIex.dylib
/usr/local/lib/libIlmThread.dylib -> /usr/local/Cellar/ilmbase/2.5.5_1/lib/libIlmThread.dylib
==> Summary
🍺  /usr/local/Cellar/openexr/3.0.3: 176 files, 5.3MB
Removing: /usr/local/Cellar/openexr/2.5.5... (152 files, 6.9MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/openexr--2.5.5.big_sur.bottle.tar.gz... (3MB)
==> Upgrading librsvg 2.50.3 -> 2.50.5 
==> Downloading https://ghcr.io/v2/homebrew/core/librsvg/manifests/2.50.5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/librsvg/blobs/sha256:a02de59a2d3b1369e1f3a83b3d05bf8d763d7
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:a02de59a2d3b1369e1f3a8
######################################################################## 100.0%
==> Pouring librsvg--2.50.5.big_sur.bottle.tar.gz
==> /usr/local/opt/gdk-pixbuf/bin/gdk-pixbuf-query-loaders --update-cache
🍺  /usr/local/Cellar/librsvg/2.50.5: 48 files, 148.6MB
Removing: /usr/local/Cellar/librsvg/2.50.3... (48 files, 141.5MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/librsvg--2.50.3.big_sur.bottle.tar.gz... (38.3MB)
==> Upgrading mysql 8.0.23_1 -> 8.0.25_1 
==> Downloading https://ghcr.io/v2/homebrew/core/libevent/manifests/2.1.12
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libevent/blobs/sha256:45758b448d82b82b6bea52bc9a72593ef22f
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:45758b448d82b82b6bea52
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/lz4/manifests/1.9.3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/lz4/blobs/sha256:7024d0b6ee857352cbd3138f752496b87fa27252a
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:7024d0b6ee857352cbd313
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/six/manifests/1.16.0_1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/six/blobs/sha256:6068e58ff59ea70f491671ad3257b129ed7d5b90a
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:6068e58ff59ea70f491671
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/protobuf/manifests/3.17.0_1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/protobuf/blobs/sha256:854c7a9b9eb7db2b9bd43a0946b3569c5943
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:854c7a9b9eb7db2b9bd43a
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/zstd/manifests/1.5.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/zstd/blobs/sha256:eae17621cfc664d6e527a6d6aa6a000343eced0f
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:eae17621cfc664d6e527a6
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mysql/manifests/8.0.25_1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mysql/blobs/sha256:db388d333de4224dcc9ca54917069c75805801f
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:db388d333de4224dcc9ca5
######################################################################## 100.0%
==> Installing dependencies for mysql: libevent, lz4, six, protobuf and zstd
==> Installing mysql dependency: libevent
==> Pouring libevent--2.1.12.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/libevent/2.1.12: 57 files, 2MB
==> Installing mysql dependency: lz4
==> Pouring lz4--1.9.3.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/lz4/1.9.3: 22 files, 657.8KB
==> Installing mysql dependency: six
==> Pouring six--1.16.0_1.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/six/1.16.0_1: 20 files, 122.7KB
==> Installing mysql dependency: protobuf
==> Pouring protobuf--3.17.0_1.big_sur.bottle.tar.gz
==> Caveats
Emacs Lisp files have been installed to:
  /usr/local/share/emacs/site-lisp/protobuf
==> Summary
🍺  /usr/local/Cellar/protobuf/3.17.0_1: 206 files, 17.8MB
==> Installing mysql dependency: zstd
==> Pouring zstd--1.5.0.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/zstd/1.5.0: 31 files, 3.5MB
==> Installing mysql
==> Pouring mysql--8.0.25_1.big_sur.bottle.tar.gz
==> Caveats
We've installed your MySQL database without a root password. To secure it run:
    mysql_secure_installation

MySQL is configured to only allow connections from localhost by default

To connect run:
    mysql -uroot

To have launchd start mysql now and restart at login:
  brew services start mysql
Or, if you don't want/need a background service you can just run:
  mysql.server start
==> Summary
🍺  /usr/local/Cellar/mysql/8.0.25_1: 300 files, 293.6MB
Removing: /usr/local/Cellar/mysql/8.0.23_1... (298 files, 297.7MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/mysql--8.0.23_1... (81.2MB)
==> Upgrading graphviz 2.46.1 -> 2.47.1 
==> Downloading https://ghcr.io/v2/homebrew/core/gd/manifests/2.3.2
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/0928fd7c0eb6a0eb181e645e2bfc8dcae3f6a70ec967f7c144fa4c094e473d7f--gd-2.3.2.bottle_manifest.json
==> Downloading https://ghcr.io/v2/homebrew/core/gd/blobs/sha256:2c746f463d1b0ceaa2a9986b9ace87da6ec8b99b1a
Already downloaded: /Users/inamurateppei/Library/Caches/Homebrew/downloads/c916f0f4390cc33b4a8220e09f9d069e1ca0368c107d517ebda67890c1ebbb05--gd--2.3.2.big_sur.bottle.tar.gz
==> Downloading https://ghcr.io/v2/homebrew/core/libtool/manifests/2.4.6_3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libtool/blobs/sha256:a70ed5b9d74ec3b06bfc202ab36491c3ecd3d
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:a70ed5b9d74ec3b06bfc20
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/graphviz/manifests/2.47.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/graphviz/blobs/sha256:41c4fe36cca429a201173d6f282bbc3e12ac
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:41c4fe36cca429a201173d
######################################################################## 100.0%
==> Installing dependencies for graphviz: gd and libtool
==> Installing graphviz dependency: gd
==> Pouring gd--2.3.2.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/gd/2.3.2: 35 files, 1.4MB
==> Installing graphviz dependency: libtool
==> Pouring libtool--2.4.6_3.big_sur.bottle.tar.gz
==> Caveats
In order to prevent conflicts with Apple's own libtool we have prepended a "g"
so, you have instead: glibtool and glibtoolize.
==> Summary
🍺  /usr/local/Cellar/libtool/2.4.6_3: 71 files, 3.7MB
==> Installing graphviz
==> Pouring graphviz--2.47.1.big_sur.bottle.tar.gz
🍺  /usr/local/Cellar/graphviz/2.47.1: 301 files, 8.2MB
Removing: /usr/local/Cellar/graphviz/2.46.1... (462 files, 12.2MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/graphviz--2.46.1.big_sur.bottle.tar.gz... (6.7MB)
==> Upgrading gd 2.3.2 -> 2.3.2 
Removing: /usr/local/Cellar/gd/2.3.1... (34 files, 1.4MB)
Removing: /Users/inamurateppei/Library/Caches/Homebrew/gd--2.3.1.big_sur.bottle.tar.gz... (300.9KB)
==> Upgrading tfenv 2.0.0 -> 2.2.2 
==> Downloading https://ghcr.io/v2/homebrew/core/tfenv/manifests/2.2.2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/tfenv/blobs/sha256:bbf7732d73d27dd91579c827b60a55674515a96
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:bbf7732d73d27dd91579c8
######################################################################## 100.0%
Error: Cannot install tfenv because conflicting formulae are installed.
  terraform: because tfenv symlinks terraform binaries

Please `brew unlink terraform` before continuing.

Unlinking removes a formula's symlinks from /usr/local. You can
link the formula again after the install finishes. You can --force this
install, but the build may fail or cause obscure side effects in the
resulting software.
inamurateppei@mbp ~ % brew unlink terraform
Unlinking /usr/local/Cellar/terraform/0.14.3... 1 symlinks removed.
inamurateppei@mbp ~ % brew install pyenv zlib bzip2 readline
Warning: pyenv 1.2.27 is already installed and up-to-date.
To reinstall 1.2.27, run:
  brew reinstall pyenv
Warning: readline 8.1 is already installed and up-to-date.
To reinstall 8.1, run:
  brew reinstall readline
==> Downloading https://ghcr.io/v2/homebrew/core/zlib/manifests/1.2.11
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/zlib/blobs/sha256:b95aa332dfc7c6dfb5e86fd30068f78e2cf87ee0
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:b95aa332dfc7c6dfb5e86f
######################################################################## 100.0%
==> Pouring zlib--1.2.11.big_sur.bottle.tar.gz
==> Caveats
zlib is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

For compilers to find zlib you may need to set:
  export LDFLAGS="-L/usr/local/opt/zlib/lib"
  export CPPFLAGS="-I/usr/local/opt/zlib/include"

For pkg-config to find zlib you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/zlib/lib/pkgconfig"

==> Summary
🍺  /usr/local/Cellar/zlib/1.2.11: 12 files, 413.6KB
==> Downloading https://ghcr.io/v2/homebrew/core/bzip2/manifests/1.0.8-1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/bzip2/blobs/sha256:e3809e379c13b3af3e18e3533f54e7bdee1c630
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:e3809e379c13b3af3e18e3
######################################################################## 100.0%
==> Pouring bzip2--1.0.8.big_sur.bottle.1.tar.gz
==> Caveats
bzip2 is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have bzip2 first in your PATH, run:
  echo 'export PATH="/usr/local/opt/bzip2/bin:$PATH"' >> ~/.zshrc

For compilers to find bzip2 you may need to set:
  export LDFLAGS="-L/usr/local/opt/bzip2/lib"
  export CPPFLAGS="-I/usr/local/opt/bzip2/include"

==> Summary
🍺  /usr/local/Cellar/bzip2/1.0.8: 26 files, 532.9KB
==> Caveats
==> zlib
zlib is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

For compilers to find zlib you may need to set:
  export LDFLAGS="-L/usr/local/opt/zlib/lib"
  export CPPFLAGS="-I/usr/local/opt/zlib/include"

For pkg-config to find zlib you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/zlib/lib/pkgconfig"

==> bzip2
bzip2 is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have bzip2 first in your PATH, run:
  echo 'export PATH="/usr/local/opt/bzip2/bin:$PATH"' >> ~/.zshrc

For compilers to find bzip2 you may need to set:
  export LDFLAGS="-L/usr/local/opt/bzip2/lib"
  export CPPFLAGS="-I/usr/local/opt/bzip2/include"

inamurateppei@mbp ~ % eval "$(pyenv init -)"
inamurateppei@mbp ~ % CPPFLAGS="-I$(brew --prefix openssl)/include -I$(brew --prefix bzip2)/include -I$(brew --prefix readline)/include -I$(brew --prefix zlib)/include" LDFLAGS="-L$(brew --prefix openssl)/lib -L$(brew --prefix readline)/lib -L$(brew --prefix zlib)/lib -L$(brew --prefix bzip2)/lib" pyenv install 3.9.0
python-build: use openssl@1.1 from homebrew
python-build: use readline from homebrew
Downloading Python-3.9.0.tar.xz...
-> https://www.python.org/ftp/python/3.9.0/Python-3.9.0.tar.xz
Installing Python-3.9.0...
python-build: use readline from homebrew
python-build: use zlib from xcode sdk
Installed Python-3.9.0 to /Users/inamurateppei/.pyenv/versions/3.9.0

inamurateppei@mbp ~ % pyenv versions
* system (set by /Users/inamurateppei/.pyenv/version)
  3.9.0
inamurateppei@mbp ~ % pyenv global 3.9.0
inamurateppei@mbp ~ % python --version
Python 2.7.16
inamurateppei@mbp ~ % pyenv global 3.9.0
inamurateppei@mbp ~ % python --version  
Python 2.7.16
inamurateppei@mbp ~ % pyenv install 3.9.0
pyenv: /Users/inamurateppei/.pyenv/versions/3.9.0 already exists
continue with installation? (y/N) N
inamurateppei@mbp ~ % python3 -v
import _frozen_importlib # frozen
import _imp # builtin
import '_thread' # <class '_frozen_importlib.BuiltinImporter'>
import '_warnings' # <class '_frozen_importlib.BuiltinImporter'>
import '_weakref' # <class '_frozen_importlib.BuiltinImporter'>
import '_io' # <class '_frozen_importlib.BuiltinImporter'>
import 'marshal' # <class '_frozen_importlib.BuiltinImporter'>
import 'posix' # <class '_frozen_importlib.BuiltinImporter'>
import '_frozen_importlib_external' # <class '_frozen_importlib.FrozenImporter'>
# installing zipimport hook
import 'time' # <class '_frozen_importlib.BuiltinImporter'>
import 'zipimport' # <class '_frozen_importlib.FrozenImporter'>
# installed zipimport hook
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/__init__.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__init__.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/__init__.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/codecs.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/codecs.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/codecs.cpython-39.pyc'
import '_codecs' # <class '_frozen_importlib.BuiltinImporter'>
import 'codecs' # <_frozen_importlib_external.SourceFileLoader object at 0x101d8beb0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/aliases.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/aliases.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/aliases.cpython-39.pyc'
import 'encodings.aliases' # <_frozen_importlib_external.SourceFileLoader object at 0x101db5490>
import 'encodings' # <_frozen_importlib_external.SourceFileLoader object at 0x101d8bcd0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/utf_8.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/utf_8.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/utf_8.cpython-39.pyc'
import 'encodings.utf_8' # <_frozen_importlib_external.SourceFileLoader object at 0x101d8bbb0>
import '_signal' # <class '_frozen_importlib.BuiltinImporter'>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/latin_1.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/latin_1.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/encodings/__pycache__/latin_1.cpython-39.pyc'
import 'encodings.latin_1' # <_frozen_importlib_external.SourceFileLoader object at 0x101db5550>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/io.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/io.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/io.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/abc.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/abc.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/abc.cpython-39.pyc'
import '_abc' # <class '_frozen_importlib.BuiltinImporter'>
import 'abc' # <_frozen_importlib_external.SourceFileLoader object at 0x101db5a00>
import 'io' # <_frozen_importlib_external.SourceFileLoader object at 0x101db5730>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/site.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/site.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/site.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/os.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/os.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/os.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/stat.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/stat.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/stat.cpython-39.pyc'
import '_stat' # <class '_frozen_importlib.BuiltinImporter'>
import 'stat' # <_frozen_importlib_external.SourceFileLoader object at 0x101deb2b0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_collections_abc.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/_collections_abc.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_collections_abc.cpython-39.pyc'
import '_collections_abc' # <_frozen_importlib_external.SourceFileLoader object at 0x101deb340>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/posixpath.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/posixpath.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/posixpath.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/genericpath.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/genericpath.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/genericpath.cpython-39.pyc'
import 'genericpath' # <_frozen_importlib_external.SourceFileLoader object at 0x101e13970>
import 'posixpath' # <_frozen_importlib_external.SourceFileLoader object at 0x101deba60>
import 'os' # <_frozen_importlib_external.SourceFileLoader object at 0x101dcf9a0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_sitebuiltins.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/_sitebuiltins.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_sitebuiltins.cpython-39.pyc'
import '_sitebuiltins' # <_frozen_importlib_external.SourceFileLoader object at 0x101de5eb0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_bootlocale.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/_bootlocale.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/_bootlocale.cpython-39.pyc'
import '_locale' # <class '_frozen_importlib.BuiltinImporter'>
import '_bootlocale' # <_frozen_importlib_external.SourceFileLoader object at 0x101e13e20>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/types.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/types.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/types.cpython-39.pyc'
import 'types' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2fd90>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/__init__.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__init__.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/__init__.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/warnings.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/warnings.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/warnings.cpython-39.pyc'
import 'warnings' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2ecd0>
import 'importlib' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2f550>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/util.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/util.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/util.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/abc.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/abc.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/abc.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/machinery.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/machinery.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/importlib/__pycache__/machinery.cpython-39.pyc'
import 'importlib.machinery' # <_frozen_importlib_external.SourceFileLoader object at 0x101e30460>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/typing.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/typing.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/typing.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/__pycache__/__init__.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/__init__.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/__pycache__/__init__.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/heapq.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/heapq.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/heapq.cpython-39.pyc'
# extension module '_heapq' loaded from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/lib-dynload/_heapq.cpython-39-darwin.so'
# extension module '_heapq' executed from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/lib-dynload/_heapq.cpython-39-darwin.so'
import '_heapq' # <_frozen_importlib_external.ExtensionFileLoader object at 0x101e91fa0>
import 'heapq' # <_frozen_importlib_external.SourceFileLoader object at 0x101e91ac0>
import 'itertools' # <class '_frozen_importlib.BuiltinImporter'>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/keyword.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/keyword.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/keyword.cpython-39.pyc'
import 'keyword' # <_frozen_importlib_external.SourceFileLoader object at 0x101e9c160>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/operator.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/operator.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/operator.cpython-39.pyc'
import '_operator' # <class '_frozen_importlib.BuiltinImporter'>
import 'operator' # <_frozen_importlib_external.SourceFileLoader object at 0x101e9c220>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/reprlib.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/reprlib.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/reprlib.cpython-39.pyc'
import 'reprlib' # <_frozen_importlib_external.SourceFileLoader object at 0x101e9c2e0>
import '_collections' # <class '_frozen_importlib.BuiltinImporter'>
import 'collections' # <_frozen_importlib_external.SourceFileLoader object at 0x101e75f40>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/__pycache__/abc.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/abc.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/collections/__pycache__/abc.cpython-39.pyc'
import 'collections.abc' # <_frozen_importlib_external.SourceFileLoader object at 0x101e7a310>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/contextlib.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/contextlib.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/contextlib.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/functools.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/functools.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/functools.cpython-39.pyc'
import '_functools' # <class '_frozen_importlib.BuiltinImporter'>
import 'functools' # <_frozen_importlib_external.SourceFileLoader object at 0x101ea9c40>
import 'contextlib' # <_frozen_importlib_external.SourceFileLoader object at 0x101e7a520>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/re.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/re.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/re.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/enum.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/enum.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/enum.cpython-39.pyc'
import 'enum' # <_frozen_importlib_external.SourceFileLoader object at 0x101eceeb0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_compile.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/sre_compile.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_compile.cpython-39.pyc'
import '_sre' # <class '_frozen_importlib.BuiltinImporter'>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_parse.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/sre_parse.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_parse.cpython-39.pyc'
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_constants.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/sre_constants.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sre_constants.cpython-39.pyc'
import 'sre_constants' # <_frozen_importlib_external.SourceFileLoader object at 0x101f0e730>
import 'sre_parse' # <_frozen_importlib_external.SourceFileLoader object at 0x101ef9d00>
import 'sre_compile' # <_frozen_importlib_external.SourceFileLoader object at 0x101ef94c0>
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/copyreg.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/copyreg.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/copyreg.cpython-39.pyc'
import 'copyreg' # <_frozen_importlib_external.SourceFileLoader object at 0x101f1be80>
import 're' # <_frozen_importlib_external.SourceFileLoader object at 0x101e7acd0>
import 'typing' # <_frozen_importlib_external.SourceFileLoader object at 0x101e30190>
import 'importlib.abc' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2e250>
import 'importlib.util' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2f370>
# possible namespace for /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/site-packages/google
# /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sitecustomize.cpython-39.pyc matches /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/sitecustomize.py
# code object from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/sitecustomize.cpython-39.pyc'
import 'sitecustomize' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2f250>
import 'site' # <_frozen_importlib_external.SourceFileLoader object at 0x101db5a30>
Python 3.9.5 (default, May  4 2021, 03:36:27) 
[Clang 12.0.0 (clang-1200.0.32.29)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
# extension module 'readline' loaded from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/lib-dynload/readline.cpython-39-darwin.so'
# extension module 'readline' executed from '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/lib-dynload/readline.cpython-39-darwin.so'
import 'readline' # <_frozen_importlib_external.ExtensionFileLoader object at 0x101e2f160>
import 'atexit' # <class '_frozen_importlib.BuiltinImporter'>
# code object from /usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/rlcompleter.py
# created '/usr/local/Cellar/python@3.9/3.9.5/Frameworks/Python.framework/Versions/3.9/lib/python3.9/__pycache__/rlcompleter.cpython-39.pyc'
import 'rlcompleter' # <_frozen_importlib_external.SourceFileLoader object at 0x101e2eeb0>
>>> python -V
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'python' is not defined
>>> 
zsh: suspended  python3 -v
inamurateppei@mbp ~ % pyenv versions
  system
* 3.9.0 (set by /Users/inamurateppei/.pyenv/version)
inamurateppei@mbp ~ % pyenv global 3.9.0
inamurateppei@mbp ~ % zsh -l
inamurateppei@mbp ~ % python --version
Python 3.9.0
inamurateppei@mbp ~ % 
