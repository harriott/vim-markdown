vim: fdl=3:

# Vim Markdown

## About this fork
My fork of the excellent [vim-markdown](https://github.com/preservim/vim-markdown), which supplements [vim/runtime/ftplugin/markdown.vim](https://github.com/vim/vim/blob/master/runtime/ftplugin/markdown.vim).

I created this fork so that I can tweak for highlighting of a line of code immediately after a heading, which is in agreement with Pandoc's `markdown_strict` interpretation.

My tweaks are marked 'JH'.

I grab this repository with `GitHub CLI`: `gh repo clone vim-markdown`

## merging from preservim upstream

    git remote -v                                # check remote locations
    git fetch upstream                           # grab the changed upstream
    git merge upstream/master -m 'merge message' # merges in the changes
    rg HEAD                                      # ripgrep for any conflicts
    git merge --abort                            # undo the merge

## License copied over
The MIT License (MIT)

Copyright (c) 2012 Benjamin D. Williams

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
