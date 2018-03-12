# asyncomplete-vimpire.vim

A completion source for [asyncomplete.vim](https://github.com/prabirshrestha/asyncomplete.vim)

## Install

```vim
Plug 'prabirshrestha/asyncomplete.vim'
Plug 'kotarak/asyncomplete-vimpire.vim'
```

Or use pathogen. Or vim's package.

## Register asyncomplete-vimpire.vim

```vim
au User asyncomplete_setup call asyncomplete#register_source(asyncomplete#sources#vimpire#get_source_options({
            \ 'name': 'vimpire',
            \ 'whitelist': ['clojure'],
            \ 'completor': function('asyncomplete#sources#vimpire#completor')
            \  }))
```
