# gists - show my gists

```
$ cat > /path/to/git_token
username:XXXXXXXXXXXXXXXXXXXXXXX
$ export GIT_TOKEN_FILE=/path/to/git_token
$ gists
```

```
usage: gists <[options]...>

positional arguments:
  args

optional arguments:
  -h, --help
  -d REGEX_FOR_DESCRIPTION, --dgrep REGEX_FOR_DESCRIPTION
  -f REGEX_FOR_FILENAME, --fgrep REGEX_FOR_FILENAME
  -p, --public
  -s, --secret
  -c GIST_ID, --clone GIST_ID
  -a, --all-clone
  -P FILE_NAME [-d DESCRIPTION], --push-public FILE_NAME [-d DESCRIPTION]
  -S FILE_NAME [-d DESCRIPTION], --push-secret FILE_NAME [-d DESCRIPTION]
  -F, --force           overwrite if a directory already exists
  -u, --use-ssh
  -r, --rename

```
