# dire
A viewer of dockerignore regexp.

## Installation
```
go get -u github.com/orisano/dire
```

## How to use
```
$ cat .dockerignore
foo
foo/*
bar/**
bar/**/
foobar/**/.git
foobar/a/?

$ dire
^foo$
^foo/[^/]*$
^bar/.*$
^bar/.*$
^foobar/(.*/)?\.git$
^foobar/a/[^/]$
```

## Author
Nao YONASHIRO(@orisano)
