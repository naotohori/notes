Add an existing directory.

```
$ git init

$ git remote add origin https://github.com/naotohori/XXXXX

$ git config user.name "Naoto Hori"
$ git config user.email "hori.naoto@gmail.com"

$ git fetch

$ git pull origin master

$ git add xxxx
$ git commit -m "xxxxx"

$ git push -u origin master
```


Add a (annotated) tag.

```
$ git tag -a TAGNAME -m "COMMENTS"

$ git push origin --tags
```

