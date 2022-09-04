You have to copy `css` and `js` dirs into your `vimwiki_output` folder. If
`css/style.css` ( it's defined in your own config, default is `style.css` ) is
not found, vimwiki will use the default style and copy it into `vimwiki_output`
folder ( or soft link ).

My config is below:
```vim
let g:vimwiki_list = [{
            \   'path': '~/Documents/vimwiki/',
            \   'path_html': '~/Documents/vimwiki_html/',
            \   'template_path': '~/Documents/vimwiki_template/',
            \   'template_default': 'default',
            \   'template_ext': '.html',
            \   'auto_toc': 1,
            \   'css_name': 'css/style.css'
            \   }]
```
