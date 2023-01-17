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

## Reading and Writing Files Asynchronously
Node.js’s methods for reading and writing files. Along the way we’ll see two common error-handling patterns in Node.js:
error events on EventEmitters and err callback arguments.
There are a few approaches to reading and writing files in Node. The simplest
is to read in or write out the entire file at once. This technique works well for
small files. Other approaches read and write by creating Streams or staging
content in a Buffer.
### Writing Files Asynchronously
```shell
$ node write-simple.js
```
### Reading Files Asynchronously
```shell
$ node read-simple.js
```
### Creating Read and Write Streams
The cat.js uses a file stream to pipe a file’s data to standard output:
```shell
$ chmod +x cat.js
$ ./cat.js target.txt
```
You can also listen for data events from the file stream instead of calling pipe(). The following program called read-stream.js does this:
```shell 
read-stream.js no-such-file
$ node 
```
Example of how to read a file using the readFileSync() method:
```js
const fs = require('fs');
const data = fs.readFileSync('target.txt');
process.stdout.write(data.toString());
```
