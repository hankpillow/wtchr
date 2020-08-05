## wtchr

Tiny bash script to watch for file changes and trigger another command.

> The changes captured won't be sent to the trigger!

The command uses `find` to list all files in the target folder.


## Usage:

```
$ wtchr tmp/ "echo changed!"
```

Using ignore pattern

```
$ wtchr "tmp/" "echo changed!" '-not -path "*.md"'
```

> see `find` manual to send any extra argument the command.):
