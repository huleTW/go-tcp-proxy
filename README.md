# tcp-proxy

A small TCP proxy written in Go

This project was intended for debugging text-based protocols. The next version will address binary protocols.

## Install

**Source**

``` sh
$ go get -v github.com/huleTW/go-tcp-proxy/cmd/tcp-proxy
```

## Usage

```
$ tcp-proxy --help
Usage of tcp-proxy:
  -c: output ansi colors
  -h: output hex
  -l="localhost:9999": local address
  -n: disable nagles algorithm
  -r="localhost:80": remote address
  -match="": match regex (in the form 'regex')
  -replace="": replace regex (in the form 'regex~replacer')
  -v: display server actions
  -vv: display server actions and all tcp data
```

*Note: Regex match and replace*
**only works on text strings**
*and does NOT work across packet boundaries*
