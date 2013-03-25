golang: readline 
=================

[![Build Status](https://travis-ci.org/jprichardson/commander-go.png)](https://travis-ci.org/jprichardson/ommander-go)

Easily read lines from a stream such as `stdin` for a file. Supports either `\n`, `\r\n`, or mixed.


Why?
----

Because [bufio.ReadLine()](http://golang.org/pkg/bufio/#Reader.ReadLine) is not flexible enough.



Installing
----------

    go get -u github.com/jprichardson/readline-go


Usage
-----

```go
import (
    "readline"
    "fmt"
)

readline.ReadLine(os.Stdin, func(line string) {
    fmt.Printf("Line: %s\n", line)
})
```


License (MIT)
-------------
Copyright (c) 2013 JP Richardson


Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.