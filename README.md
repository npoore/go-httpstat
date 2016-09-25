# go-httpstat

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)][license]
[![Go Documentation](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)][godocs]

[license]: https://github.com/tcnksm/go-httpstat/blob/master/LICENSE
[godocs]: http://godoc.org/github.com/tcnksm/go-httpstat

`go-httpstat` is a golang pacakge to trace HTTP latency infomation (DNSLookup, TCP Connection and so on) on any golang HTTP request. It uses [`httptrace`](https://golang.org/pkg/net/http/httptrace/) internally. Just create `go-httpstat` powered `context` and give it your `http.Request` (no big code modification is required). The original idea came from [`httpstat`](https://github.com/reorx/httpstat) command ( and Dave Cheney's [golang implementation](https://github.com/davecheney/httpstat) 👏. This package now traces same latency infomation as them.

See example usage on [example](/_example) directory. 

## Install 

Use `go get`,

```bash
$ go get github.com/tcnksm/go-httpstat
```

## Author

[Taichi Nakashima](https://github.com/tcnksm)