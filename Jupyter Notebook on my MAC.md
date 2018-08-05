This is a preq to getting Jupyter Notebook going

```bash
$ brew install pyenv-virtualenv
 
#apped to .bash_profile
if which pyenv > /dev/null; then
  eval "$(pyenv init -)"
fi
 
if which pyenv-virtualenv-init > /dev/null; then
  eval "$(pyenv virtualenv-init -)";
fi
 
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pip completion --bash)"

$ pyenv install 3.6.6
$ pyenv virtualenv 3.6.6 jupyter3
$ pyenv activate jupyter3
$ pip install ipykernel
 
$ git clone https://github.com/WillKoehrsen/Data-Analysis.git
$ cd Data-Analysis/stocker
$ mkvirtualenv stocker-test
$ cat requirements.txt
quandl==3.3.0
matplotlib==2.1.1
numpy==1.14.0
fbprophet==0.2.1
pystan==2.17.0.0
pandas==0.22.0
pytrends==4.3.0
jupyter
$ pip install -r requirements.txt
$ jupyter notebook
```