# nvim and vim

-------------
## use nvim with lazy and lua

1、解压 nvim 文件到 C:/user/<用户名>/AppData/Local

2、打开 power shell 输入 nvim 加载配置文件


🤔🤔🤔

下面是关于使用nvim和vim及其插件遇见问题的修复


1、由于版本问题导致在 python(可能还包括其他语言) 程序中无法使用Tab键：
解决方法：

在 nvim 的配置文件 init.vim 写入一下两行：
```
inoremap <expr> <Tab> pumvisible() ? "\<C-n>" : "\<Tab>"
inoremap <expr> <S-Tab> pumvisible() ? "\<C-p>" : "\<S-Tab>"
```



