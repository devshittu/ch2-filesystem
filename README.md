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

## Reading Command-Line Arguments
```shell
$ node watcher-argv.js target.txt
```

## Spawning a Child Process

Enhancing our file-watching example program even further by having it spawn a child process in response to a change.

```shell
$ node watcher-spawn.js target.txt
```


## Capturing Data from an EventEmitter
Sometimes you’ll want to capture data from a stream, rather than just piping it forward. Let’s see how to do that in capturing data from an EventEmitter

```shell
$ node watcher-spawn-parse.js target.txt
```

## 

```shell
$ node 
```

## 

```shell
$ node 
```