# accepter

[![GoDoc](https://godoc.org/github.com/orkunkaraduman/go-accepter?status.svg)](https://godoc.org/github.com/orkunkaraduman/go-accepter)

Package accepter provides an Accepter and utilities for net.Listener.
It is similar with GoLang's http.Server.

## Changes from v1

* using cancelling context instead of channel
* changed Handler.Serve arguments to (ctx, conn) from (conn, closeCh)
* removed panic recovering for Handler.Serve(...)
* removed Accepter.ErrorLog
