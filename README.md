# gists - show my gists

## Install

```
$ cargo install ripgrep # brew install ripgrep
$ gem install gist
$ gist --login
$ git clone https://github.com/miyagaw61/gists
$ cp -a ./gists/gists /usr/local/bin/
$ go get github.com/motemen/ghq
$ git config --global ghq.root "~/src"
$ cat > /path/to/git_token
username:XXXXXXXXXXXXXXXXXXXXXXX
$ export GIT_TOKEN_FILE=/path/to/git_token
$ pip install git+https://github.com/miyagaw61/enert
$ gists --help
$ gists
```

## Usage

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

- show all gists

```
gists
```

- show all public gists or secret gists

```
gists -p
gists -s
```

- file name grep

```
gists -f '.*md'
```

- description grep

```
gists -d 'linux'
```

- clone one gist

```
gists -c 0123456789abcdef
```

- clone some gists at once time

```
gists -s -f '.*md' --all-clone
```

- clone ( use ssh )

```
gists -s --all-clone --use-ssh
```

- push ( public )

```
gists --push-public FILENAME.md
```

- push ( secret )

```
gists --push-secret FILENAME.md
```

- update gists ( This is safe even if you have something to do. )

```
gists -s --all-clone --force
```
