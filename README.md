npm version + git flow
======================


## Prerequesites

```bash
$ git flow init
```

``.git/config``:
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


## Order of Execution

### Versioning

1. Run the **preversion** script.
2. Bump version in package.json as requested (patch, minor, major, etc).
3. Run the **version** script.
5. Commit and tag.
6. Run the **postversion** script.

### Publishing

1. prepublish: Run BEFORE the package is published.
2. publish, postpublish: Run AFTER the package is published.


---

# Fooo!!!

git flow finish release -> merges & tags
npm version -> bumps version, commits & tags
