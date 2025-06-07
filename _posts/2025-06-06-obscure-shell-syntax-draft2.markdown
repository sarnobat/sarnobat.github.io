layout: post
title: "Obscure Shell Syntax"
date: 2025-06-06
categories: shell

# Obscure Shell Syntax

(this layout might be better: https://github.com/dylanaraps/pure-sh-bible?tab=readme-ov-file#default-value )
2025-03-15: improve on this: https://gist.github.com/ClementNerma/1dd94cb0f1884b9c20d1ba0037bdcde2

### !number

* `!:0`
* `!:1`
* `!:1-3`
* `!:1-`
* `!#1`

### !symbol

* `!$`
* `!^`
* `!*`
* `!#`

### !!operation

* `!!`
* `!!:p`
* `!!:s/foo/bar/`
* `!!:gs/foo/bar/`

### !<prefix>

* `!ls`
* `!ls:3`

## 
###
* `$PWD`
* `${PWD}`
* `${PWD:gs/Users/home/}`
* `${PWD:s/Users/home/}`
* `"${PWD:/$HOME/~/}"`
* `${PWD:3:5}`

###

* `${FILE:-/tmp/in.txt}`
* `${FILE:=/tmp/in.txt}`

###
* `${1:"fallback_value"}`
* `${1:-"fallback_value"}`
* `${1:+"value_if_set"}`
* `${1:?"missing argument. Exiting."}`

###

* `$@`
* `$1`
* `$2`
* `$_`

###
* `$?`
* `$$`
* `$!`

###

* `""`
* `$""`
* `$''`

###

* `${PWD:l}`
* `${PWD:u}`
* `${PWD:t}`
* `${PWD:r}`
* `${PWD:t:u}`

What the end result will look like (think about if this is what you really want: https://learnxinyminutes.com/vimscript/ )