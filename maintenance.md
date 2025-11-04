vim: fdl=3:

# my personal maintenance notes
    $vfvp/packs-cp-full/opt/vim-markdown/ftdetect/markdown.vim

When sourced, replaces vim's defaults:

    $VIMRUNTIME/ftplugin/markdown.vim
    $VIMRUNTIME/syntax/markdown.vim

## merging from preservim upstream

    $vfvp/packs-cp-full/opt/vim-markdown
    gsu  # - and ensure no waiting commits
    git pull --unshallow
    git remote -v                                   # check remote locations
        git remote add upstream https://github.com/preservim/vim-markdown
    git fetch upstream                              # grab the changed upstream
    git merge upstream/master -m '9 commits behind' # merges in the changes
    rg HEAD                                         # ripgrep for any conflicts
    in vim: /^<<<<<<< HEAD$\|^=======$\|^>>>>>>> upstream/master$
    gic '9 commit behind'
    git merge --abort                               # undo the merge

modeline spacer

