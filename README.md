# alien-minimal

### Installation

Add the following line to your .zshrc depending on your zsh plugin manager

##### [antigen](https://github.com/zsh-users/antigen):

    antigen theme eendroroy/alien-minimal alien-minimal

##### [zgen](https://github.com/tarjoilija/zgen):

    zgen load eendroroy/alien-minimal

##### [zplug](https://github.com/zplug/zplug):

    zplug "eendroroy/alien-minimal"

##### [oh-my-zsh: Overriding and Adding Themes](https://github.com/robbyrussell/oh-my-zsh/wiki/Customization#overriding-and-adding-themes)

#### screencast

[![asciicast](http://asciinema.org/a/134365.png)](https://asciinema.org/a/134365)

#### customizations
    
Adding the following in .zshrc:

    export PROMPT_START_TAG='-->'
    export PROMPT_END_TAG=' $'
    export PROMPT_START_TAG_COLOR=81
    export PROMPT_END_TAG_COLOR=81

Will make the prompt look like:

     --> ~ $
     --> ~ $ 1
    (venv) --> python-project $
    (venv) --> python-project $ 130

You can additionally show the error color on prompt start tag:

    export AM_ERROR_ON_START_TAG=1

Note: if `PROMPT_START_TAG` is empty, this configuration will be ignored.

Show versions:

Available version are: `RUBY` `PYTHON` `JAVA`
Prompt maintain declaration order.

    export AM_VERSIONS_PROMPT=(RUBY PYTHON JAVA)

Use 8 bit color:

    export AM_USER_TERMINAL_COLOR=1

Show time for each process:

    export AM_SHOW_PROCESS_TIME=0 # hide
    export AM_SHOW_PROCESS_TIME=1 # show
    export AM_SHOW_PROCESS_TIME=2 # show if not 0

Configure dirname in prompt:

    export AM_SHOW_FULL_DIR=1 # shows the full dir path
    export AM_SHOW_FULL_DIR=0 # shows the current dir name

Update left prompt asynchrononusly (initially show full directory path, update to short form later, this is just a fancy option)

    export AM_UPDATE_L_PROMPT=1

Note: this overrides `AM_SHOW_FULL_DIR` configuration

Color themes:

    1. export AM_THEME=MONO
    2. export AM_THEME=MONO_BRIGHT

#### libs

['256color'](https://github.com/chrissicool/zsh-256color) by **[@chrissicool](https://github.com/chrissicool)**

['zsh-async'](https://github.com/mafredri/zsh-async) by **[@mafredri](https://github.com/mafredri)**

['promptlib-zsh'](https://github.com/eendroroy/promptlib-zsh) by **[@eendroroy](https://github.com/eendroroy)**

