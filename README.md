# gists - show my all gists

```
$ cat > /path/to/git_token
username:XXXXXXXXXXXXXXXXXXXXXXX
$ export GIT_TOKEN_FILE=/path/to/git_token
$ gists
```

```
usage: gists [-d|--dgrep=REGEX_FOR_DESCRIPTION] [-f|--fgrep=REGEX_FOR_FILENAME] [-p|--public] [-s|--secret] [-c|--clone=GIST_HASH]

positional arguments:
  args

optional arguments:
  -h, --help
  -d DGREP, --dgrep DGREP
  -f FGREP, --fgrep FGREP
  -p, --public
  -s, --secret
  -c CLONE, --clone CLONE
```
