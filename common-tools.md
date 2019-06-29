

### virtualenvwrapper
install

    $ pip install virtualenvwrapper
    ...
    $ export WORKON_HOME=~/Envs
    $ mkdir -p $WORKON_HOME
    $ source /usr/local/bin/virtualenvwrapper.sh
    $ source ~/.local/bin/virtualenvwrapper.sh (for ubuntu18+)

list available environments

    workon
    workon env1
    
source env1/bin/activate

deactivate

rmvirtualenv venv

