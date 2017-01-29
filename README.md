# gommand
 
Go one liner program similar to python -c
 
## How can I get it?

```
go get github.com/sno6/gommand
```

=======
## Examples 
 
Write any Go code in a single line context, gommand will handle your imports and main function for you.

```gommand 'fmt.Println("Hello gommand")'``` 

or short version:

```gommand 'p("Hello, World!")'```

You could also quickly serve your current directory in one line.
 
```gommand 'http.Handle("/", http.FileServer(http.Dir("."))); fmt.Println(http.ListenAndServe(":8080", nil))'```

Dump any var/struct/slice (github.com/k0kubun/pp must be installed)

```gommand 'pp(os.Environ(), os.Args[1:])' 1 2```

Quickly find the date.

```gommand 'fmt.Println(time.Now())'```
