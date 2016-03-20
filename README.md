# zlib-cli
Simple CLI utility for the zlib compression format

Contains two complementary CLI utilities, one for compressing, the other
for uncompressing i.e `zlib-compress` and `zlib-uncompress`.

* Note:
Both utils:
- Read either from stdin or from a file on disk passed in as a path.
- Output their result to stdout.


### Installation and usage

- zlib-compress

CLI utility to compress data in the zlib format.
It takes in either a source file or content from stdin e.g

```shell
$ go get github.com/odeke-em/zlib-cli/cmd/zlib-compress
$ cat content | zlib-compress > output.compressed
$ zlib-compress ~/Downloads/fileUp > output.compressed
```

- zlib-uncompress

```shell
$ go get github.com/odeke-em/zlib-cli/cmd/zlib-uncompress
$ cat content.compressed | zlib-uncompress > uncompressed
$ zlib-uncompress content.compressed > uncompressed
```
