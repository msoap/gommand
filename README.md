# gommand
 
Go one liner program similar to python -c
 
## How can I get it?

```
go get github.com/sno6/gommand
```

Usage
-----
```bash
gommand 'fmt.Println("Hello, World!")'
```

or short version:

```bash
gommand 'p("Hello, World!")'
```

You can quickly write and run code without worrying about setting up a go file.
gommand auto imports whatever packages are being used by the program so you don't have to worry about it.
=======
## Examples 
 
Write any Go code in a single line context, gommand will handle your imports and main function for you.

```gommand 'fmt.Println("Hello gommand")'``` 

You could also quickly serve your current directory in one line.
 
```gommand 'http.Handle("/", http.FileServer(http.Dir("."))); fmt.Println(http.ListenAndServe(":8080", nil))'```

Dump any var/struct/slice (github.com/k0kubun/pp must be installed)

```gommand 'pp(os.Environ(), os.Args[1:])' 1 2```

Quickly find the date.

```gommand 'fmt.Println(time.Now())'```
