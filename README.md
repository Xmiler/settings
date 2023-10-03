# env
```
sudo apt install bash-completion && mkdir ~/.bash_completion.d && curl https://raw.githubusercontent.com/cykerway/complete-alias/master/complete_alias > ~/.bash_completion.d/complete_alias && source ~/.bash_completion.d/complete_alias
```

# bash
```
# ~/.bashrc

alias l="ls -1"
alias g="git"
alias p="python"
```
post-configure
```
for X in l g p; do complete -F _complete_alias $X; done && source ~/.bash_completion.d/complete_alias
```


# git

```
# ~/.gitconfig

[alias]
        st = status
        hist = log --pretty=format:'%C(white)%h %C(yellow)%cd %C(blue)%ce: %C(green)%s' --date=format:'%y-%m-%d %H:%M' -n20
	df = diff
	dfs = diff --staged
	ch = checkout
	cm = commit -m
```
