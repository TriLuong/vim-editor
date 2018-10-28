# Vim_editor
-----
<h3>
Search and Replace
</h3>

Find each occurrence of 'foo' (in all lines), and replace it with 'bar'.     
    
    :%s/foo/bar/g


Find each occurrence of 'foo' (in the current line only), and replace it with 'bar'. 

    :s/foo/bar/g


Change each 'foo' to 'bar', but ask for confirmation first. 

    :%s/foo/bar/gc


Change only whole words exactly matching 'foo' to 'bar'; ask for confirmation. 

    :%s/\<foo\>/bar/gc


Change each 'foo' (case insensitive due to the i flag) to 'bar'; ask for confirmation. 
:%s/foo\c/bar/gc is the same because \c makes the search case insensitive. 
This may be wanted after using :set noignorecase to make searches case sensitive (the default). 

    :%s/foo/bar/gci


Change each 'foo' (case sensitive due to the I flag) to 'bar'; ask for confirmation. 
:%s/foo\C/bar/gc is the same because \C makes the search case sensitive. 
This may be wanted after using :set ignorecase to make searches case insensitive. 

    :%s/foo/bar/gcI
--------------
<h3>
Reference:
</h3>
http://vim.wikia.com/wiki/Search_and_replace
