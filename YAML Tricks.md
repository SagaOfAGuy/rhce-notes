# Configure VIM for YAML files (Tabs) 

https://www.reddit.com/r/redhat/comments/j92xmw/ultimate_vim_tips_and_tricks_for_exam/

Other Vim tricks - https://superuser.com/questions/285500/how-to-run-unix-commands-from-within-vim

vim configuration file location: /etc/vimrc

1. Add the following line in vim : 

```
echo "set ts=2 sw=2 expandtab" >> /etc/vimrc
```

2. Add the following in vim : 

```
echo "set paste" >> /etc/vimrc
```
3. Add the following in vim : 

```
echo "set number" >> /etc/vimrc
```
