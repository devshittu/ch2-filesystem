# ch2-filesystem
N8TRW: access a filesystem: reading, writing, renaming, and deleting files.


Since you’ll be touching the target file a lot to trigger changes automatically, you might want to use the watch command to do this automatically:

```shell
$ watch -n 1 touch target.txt
```

Run launch the watcher program using node, like so:

```shell
$ node watcher.js
```

##Reading Command-Line Arguments
```shell
$ node watcher-argv.js target.txt
```

##Spawning a Child Process

Enhancing our file-watching example program even further by having it spawn a child process in response to a change.

```shell
$ node watcher-spawn.js target.txt
```




```shell
$ node 
```