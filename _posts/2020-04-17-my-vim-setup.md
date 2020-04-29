---
layout: "post"
title: "My VIM Setup"
date: 2020-04-17
category: Dev
tags: [vim, jekyll]
---

![image-title-here](/assets/images/mt-ruapehu-desert-drive.jpg){:class="img-fluid"}
*Mt. Ruapehu in Desert Road Scenic Drive*  

When I first tried VIM maybe 5 years ago. I taught that I wouldn't able to learn. It's very hard at first memorizing the keystroke using only keyboard. I remember in my last job, I tried to edit a file using VIM and I messed up, fortunately I remember to quit without saving `q!`. Right now, I can say that I am more confident than 5 years ago.

The one thing that I liked VIM is that if you start learning and embrace the beauty on it, you will never stop trying until you will become an expert. I will share with you my personal VIM setup in my machine. 

## The ColorScheme 
I'm using badwolf because of it's dark UI with distinquish colors. To install, just `git clone https://github.com/sjl/badwolf.git` and put in the ~/.vim/colors folder. Now, edit the .vimrc and add  
```
colorscheme badwolf
```
restart vim and see the changes. See also, sample from [here](http://vimcolors.com/3/badwolf/dark){:target="_blank"}

## The NERDTree
The NERDTree is a file system explorer for the VIM. It is plugin that you can install and help you visualize the directory while you are coding. It's like windows explorer. I have been struggling last time when opening a file and switch to another file. It's not only time consuming but also irritating. Feel me? So, I started to find solution in my problem and I found NERDTree. The installation is a little bit confusing at first. 

**There are steps to install NERDTree**
1. Install Pathogen.VIM first (help you to install plugin)
* mkdir ~/.vim/autoload
* curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim
2. Add this below to .vimrc
```
execute pathogen#infect()
syntax on
filetype plugin indent on
```
3. Download NERDTree
* mkdir ~/.vim/bundle
* git clone https://github.com/preservim/nerdtree.git ~/.vim/bundle/nerdtree

![alt text][nerdtree]{:class="img-fluid"}
you can find more tutorial from [vimawesome.com](https://vimawesome.com/plugin/nerdtree-red){:target="_blank"}

To make your life easier, add this line to your .vimrc and after typing vim you can just execute `<ctrl-n>` instead of typing NERDTree.
```
map <C-n> :NERDTreeToggle<CR>
```
## The NERDCommenter

From the root word "comment", yeah you heard it right! This is all about commenting your code in a VIM'ish way. The first time I use it I was impressed how it know what kind of comment you are executing. Like, if your code is python it will change the comment symbol to `#` and if you change to html it will use the `<!-- -->` symbol.

**How to install**
1. go to ~/.vim/bundle and git clone `https://github.com/preservim/nerdcommenter.git`.
2. add this to ~/.vimrc
```
filetype plugin on
set mapleader=","
```
changing the mapleader to `,` makes it easy to execute the command. By pressing `, cc` you able comment the code. You find more information [here](https://github.com/preservim/nerdcommenter){:target="_blank"}


That's all folks! Just keep on trying as Roy T. Bennett said 
<blockquote class="blockquote">"Do not fear failure but rather fear not trying"</blockquote>

[nerdtree]: /assets/images/nerdtree-vim.png
