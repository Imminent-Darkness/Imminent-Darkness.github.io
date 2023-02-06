---
menutitle:         "Introduction to Sed"
description:       "Short introduction to Sed."
category:          Tutorials
author:            "Steven Wilkins"
tags:              Sed Linux Tools Tutorial
---

{% include navigation.html %}

# Introduction to Sed 

`sed`, short for Stream Editor, is a powerful command-line tool for transforming text. It is a non-interactive text editor that is used to perform basic text transformations, such as replacing text, deleting text, or printing specific lines of a file. This tool is very useful for text manipulation and is widely used in shell scripts and data processing.

## Basic Usage

The basic syntax of `sed` is as follows:

```bash 
sed 's/old-text/new-text/g' input-file
```

Where `s/old-text/new-text/g` is the command for replacing `old-text` with `new-text`, and `g` at the end of the command specifies that the operation should be performed globally (i.e. on all instances of `old-text`). The `input-file` argument is the file on which you want to perform the text transformation.

For example, to replace all occurrences of the word "apple" with the word "banana" in the file `fruits.txt`, you would run the following command:

```bash 
sed 's/apple/banana/g' fruits.txt
```

This would output the transformed text to the terminal, but it would not modify the original file. To actually save the changes to the file, you would need to use the `-i` or `--in-place` option, like so:

```bash 
sed -i 's/apple/banana/g' fruits.txt
```

## Advanced Usage

`sed` can also be used for more advanced text transformations, such as printing specific lines of a file. The basic syntax for printing specific lines is as follows:

```bash 
sed -n '3,5p' input-file
```

This command would print lines 3 to 5 of the `input-file`. Note the use of the `-n` option, which prevents `sed` from automatically printing each line of the file. The `p` at the end of the command specifies that the specified lines should be printed.

Another useful feature of `sed` is the ability to perform multiple operations in a single command. For example, you could replace the word "apple" with "banana" and then delete all lines containing the word "pear" with the following command:

```bash 
sed -i 's/apple/banana/g; /pear/d' fruits.txt
```

## Conclusion 

`sed` is a powerful and flexible tool for text transformations. Whether you need to replace a single word, print specific lines, or perform complex text manipulations, `sed` can help you get the job done quickly and efficiently. With its concise syntax and wide range of capabilities, `sed` is an essential tool for any data processing or shell scripting work.
