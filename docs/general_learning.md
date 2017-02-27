## Setup
Visual Studio Code provides decent DX with little overhead...

See [Go Tooling in Action](https://www.youtube.com/watch?v=uBjoTxosSys&feature=youtu.be) for a preview of what is possible!

my key shortcuts to run tests:

// Place your key bindings in this file to overwrite the defaults
[
    {   "key": "cmd+shift+enter",
        "command": "go.test.file",
        "when": "editorFocus && editorLangId == 'go'" }
]


## Collection of starter material:

  https://github.com/gophersgang


## getting a package to run:

in GOPATH with proper folders ... sigh... (like github.com/mindreframer/...)

    $ go get -t -v ./...
    $ go test -v ./...


## Learning:
  - https://www.golang-book.com/guides/bootcamp/ -> fucking good!!!
  - https://www.goin5minutes.com/screencasts/ (Short Screencasts)
  - https://s905060.gitbooks.io/site-reliability-engineer-handbook/go_file_operations.html (from Google)
  - https://www.youtube.com/channel/UC_BzFbxG2za3bp5NRRRXJSw (JustForFunc channel with Golang videos)


## Examples
  - [Working with Files in Go - 2015](http://www.devdungeon.com/content/working-files-go)
  - [Packet Capture - 2015](http://www.devdungeon.com/content/packet-capture-injection-and-analysis-gopacket)


## Streams
  - [Advanced Patterns with io.ReadWriter](http://www.slideshare.net/weaveworks/advanced-patterns-with-ioreadwriter)


## Courses:
  - https://github.com/golang/go/wiki/Courses
