+++
title = 'Vim Essentials'
date = 2024-10-02T21:22:48+02:00
draft = true
+++

# Vim Essentials

## Vim Deleting
`x` to delete char over cursor
`X` delete backwords previous char
`D` or `D$` delete from cursor to end of line
`dw` delete from the cursor to the end of the word
`dW` delete from the cursor to the end of the word including puntuaction and space
`db` or `dB` delete backwords to the beginning of the word
`2dw` delete two words
`2dW` delete two words with puntuaction
`daw` delete to the word from the beginning even if you are not over the first char
`DD` delete whole line
`3DD` delete 3 lines

## Getting Help
`:help` to get help
`:help command` to get help for a specific commnad
`:help subject` to get help for a subject (ex `:help linewise`)
`ctrl + i` page forward, `ctrl + o` page backward
if in the documentatin type `cmd + [` search help for the word over the cursor
`ctrl + w w` toggle between help window and document window

## Cut, Copy & Paste
`d` and `x` cut text not just delete it
cut = delete and save into a register (cliboard storage)
`p` paste (put) text from register
`P` paste (put) text above the cursor (lines) or previous char
`xp` to swap char
`y` yank (copy)
`yw` copy entire word
`Y` copy from cursor to end of line
`yy` yank entire line
`yyp` duplicate line
`4yy` yank 4 lines
`u` undo last command
`ctrl r` redo

### Registers
There are 3 different types of register:
- unnamed
- numbered
- named

Registers are precedes from double quotes:
- unnamed register = ""
- numbered registers = "0 "1 ...  "9

The unnamed register "" holds text from `d`,`c`,`s`,`x` and `y` operations
`"0` holds last text yanked `y`
`"1` holds last text deleted `d` or changed `c`

numbered registers shift with each `d` or `c`

