# honkit-test

```
$ cd honkit-test
$ mkdir md docs
$ echo "# Honkit test" > ./md/README.md
$ echo "# Chapter 1" > ./md/Chapter1.md
$ echo "# Summary\n\n* [Home](README.md)\n* [Chapter 1](Chapter1.md)" > ./md/SUMMARY.md
$ npm install honkit --save-dev
$ npm install gitbook-plugin-hide-published-with --save-dev
```

```
$ cat md/book.json
{
    "title": "test",
    "plugins":[
        "hide-published-with"
    ]
}
```

```
$ npx honkit build ./md ./docs
```

