# Custom Scripts
Just a couple of scripts to make life easier.

- open `~/.bashrc` with an editor your choice
- paste the functions in the file
- then source it with source `~/.bashrc`

You are now ready to do everything from you terminal.

## Google Search
```
google() {
    search=""
    echo "Googling: $@"
    for term in $@; do
        search="$search%20$term"
    done
    xdg-open "http://www.google.com/search?q=$search"
}
```


## Leo Search
```
leo() {
    search=""
    echo "Translating: $@"
    for term in $@; do
        search="$search%20$term"
    done
    xdg-open "https://dict.leo.org/englisch-deutsch/$search
}
```
