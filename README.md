# ElfDiff

<img src="https://mjsaldanha.com/images/elf_icon.png" width="128" height="128">

So you are writing a scientific article, and your advisor often reviews it and gives you feedback about what should be changed.

You then make the changes and wants a nice way to display the changes to your advisor.

I'd say your best bet is [diffy.org](https://diffy.org/).

However, if you really really like the command line, you can use **ElfDiff** :).

# Usage

**TL;DR** Use it this way:

```
git diff --word-diff=plain > output.txt
elfdiff output.txt > output.html
firefox output.html
# OR
git diff --word-diff=plain | elfdiff > output.html
firefox output.html
```


1) Create the diff file using the following command

```
git diff --word-diff=plain > output.txt
```

2) Run ElfDiff to convert it to HTML

```
elfdiff output.txt > output.html
```

3) Check the HTML file using your browser

```
firefox output.html
```

**NOTE:** The git diff command can also be used by passing specific branches as argument. <br> Example: `git diff --word-diff=plain master^`
