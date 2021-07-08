mkdir git-alias && cd git-alias

code .

git config -global --edit


[alias]
	c = !git add --all && git commit -m
	s = !git status -s
  l = !git log --pretty=format:'%C(blue)%h %C(white)%s %C(cyan)%cn %C(green)%cr %C(red)%d'
  count = !git shortlog -s --grep
	amend = !git add --all && git commit --amend