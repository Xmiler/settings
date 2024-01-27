# .bashrc
```
# ~/.bashrc

alias l="ls -1"
memp(){
    smem -t -k -c pss -P $1 | tail -n1;
}
```


# .gitconfig

```
# ~/.gitconfig

[alias]
        st = status
        hist = log --pretty=format:'%C(white)%h %C(yellow)%cd %C(blue)%ce: %C(green)%s' --abbrev=8 --date=format:'%y-%m-%d %H:%M' -n20
	df = diff
	dfs = diff --staged
	ch = checkout
	cm = commit -m
```
