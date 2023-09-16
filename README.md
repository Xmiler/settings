# git

`~/.gitconfig`:
```
[alias]
        st = status
        hs = log --pretty=format:'%C(white)%h %C(yellow)%cd %C(blue)%ce: %C(green)%s' --date=format:'%y-%m-%d %H:%M' -n20
	df = diff
	dfs = diff --staged
	ch = checkout
	cm = commit -m
```
