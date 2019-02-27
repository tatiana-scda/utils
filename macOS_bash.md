# macOS bash
here's how to save a new alias using macOS

## open bash_profile
the terminal app runs by default .bash_profile instead of .bashrc
```
vim .bash_profile
```
or
```
vim ~/.bash_profile
```

if not familirezed with ```vim``` text editor, you can use ```open``` command and edit it using you default text editor.

## colour scheme

you can change it in many ways, play around with this basic:
```
export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]\$ "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad
```
## alias
to set an alias, save the new command without quotes, and the old command in single ones. pay attention, there's no space between the equal sign.
```
alias pip='pip3'
alias python='python3'
```

Adding jnote and a ```jupyter notebook``` alias is a bit diffent since alias command doesn't work with two words. This function will make ```jnote``` an alias. The ```$@``` means that everything after ```jnote``` will be a paramter of ```jupyter notebook``` command.
```
jnote() {
	jupyter notebook $@
}
```
