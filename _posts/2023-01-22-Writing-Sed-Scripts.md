---
menutitle:         "Writing Sed Scripts"
description:       "`sed`, short for Stream Editor, is a powerful command-line tool for transforming text. It is widely used for text 
                    manipulation and is often used in shell scripts and data processing. Writing sed scripts can make it easier to 
                    automate repetitive text transformations and improve your workflow."
category:          Tutorials
author:            "Steven Wilkins"
tags:              Sed Linux Tools Tutorial
---

{% include navigation.html %}

## Basic Structure

A `sed` script is simply a series of `sed` commands stored in a file. The basic structure of a `sed` script is as follows:

```bash 
#!/bin/sed -f

# Command 1
s/old-text/new-text/g

# Command 2
s/old-text/new-text/g

# etc.
```

The first line of the script specifies the location of the `sed` executable, and the `-f` option tells `sed` that it should read its commands from a file. The script then consists of one or more `sed` commands, each on a separate line.

## Script Variables

`sed` scripts can also include variables, which can make it easier to perform repetitive text transformations. Variables are defined using the `-e` option followed by an assignment, like so:

```bash 
#!/bin/sed -f

# Define a variable
-e 's/old-text/new-text/g'

# Use the variable in a command
s/$old-text/$new-text/g
```

This allows you to reuse the same text transformation in multiple places within the script, without having to repeat the transformation for each instance.

## Applying the Script 

Once you've written your `sed` script, you can apply it to a file using the following syntax:

```bash 
sed -f script.sed input-file
```

Where `script.sed` is the name of your `sed` script file and `input-file` is the file on which you want to perform the text transformations.

## Conclusion

Writing `sed` scripts can greatly simplify and streamline your text transformation workflows. With its concise syntax and wide range of capabilities, `sed` is a powerful tool for any data processing or shell scripting work, and writing scripts can help you take full advantage of its capabilities. Whether you need to perform simple text replacements or more complex transformations, `sed` scripts can help you get the job done quickly and efficiently.
