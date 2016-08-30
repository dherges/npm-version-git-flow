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


## Order

1. Run the **preversion** script.
2. Bump version in package.json as requested (patch, minor, major, etc).
3. Run the **version** script.
5. Commit and tag.
6. Run the **postversion** script.
