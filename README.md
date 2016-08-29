npm version + git flow
======================


```bash
$ git flow init
```

``.git/config``
```
[branch "master"]
	remote = origin
	merge = refs/heads/master
[branch "develop"]
        remote = origin
        merge = refs/heads/develop
[gitflow "branch"]
	master = master
	develop = develop
[gitflow "prefix"]
	feature = feature/
	release = release/
	hotfix = hotfix/
	support = support/
	versiontag = 
```
