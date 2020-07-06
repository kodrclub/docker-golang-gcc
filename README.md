Docker image that includes golang and gcc.

Image tags refer to the version of Golang used.

---

Usage:

- Create an alias in the form

```
alias gogcc='docker run --rm -it -v $(pwd):/app -w /app kodrclub/golang-gcc:1.14 go "$@"'
```

- Test with something like

```
$ gogcc version
```

- To build, tag and push your own version of the images to your registry, replace the username in the provided `Makefile`s and just run `make` inside the directory for the appropriate Dockerfile.
