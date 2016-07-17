# lang-server

lang-server is a simple tool that leverages zepto #langs to
build a simple framework for simple servers.

# Installation

```
zeps install hellerve/lang-server
```

# Usage

```clojure
#lang serve
; the handle function will be called with every request
(define (handle method route headers body)
  (response :body "Hello, World"))
```

After saving the file to `my-server.zp`, you can run this script using

```
zepto-serve my-server
```

For a more or less complex example leveraging a few more
possibilities, see the [example JSON server](https://github.com/hellerve/lang-server/blob/master/examples/serve-json/serve-json.zp).

<hr/>
Have fun!
