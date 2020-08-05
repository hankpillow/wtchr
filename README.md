## wtchr

Tiny bash script to watch for file changes and trigger another command.

> The changes captured won't be sent to the trigger!

The command uses `find` to list all files in the target folder.

## Install

```
curl https://raw.githubusercontent.com/hankpillow/wtchr/master/wtchr -o /usr/bin/wtchr
chmod +x /usr/bin/wtchr
```

## Usage:

```
$ wtchr tmp/ "echo changed!"
```

You can pass args to `find` command:

```
$ wtchr "tmp/" "echo changed!" '-not -path "*.md"'
```

