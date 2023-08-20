# go-tinyEQfeed
WASM implementation of a go based EQ feed

## What if go curated output from the USGS EQ feed on a webpage? 
Yes, it could be done with javascript but this is a Go experiment and a wasm learning opportunity.

### Let's see how it goes.

from https://github.com/tinygo-org/tinygo/tree/release/src/examples/wasm

-sad face- I received an error "error: requires go version 1.18 through 1.20, got go1.21"

I dug out a Toshiba laptop with Ubuntu and installed Go version 1.20.7 & TinyGo version 0.28.1; re-initialized go mod. 
```go mod init go-tinyEQfeed```

Then build the light wasm file:
```tinygo build -o go-tinyEQfeed ./go-tinyEQfeed.go```

Run to test:
```tinygo run go-tinyEQfeed.go```

