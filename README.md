## About me,
- 😄 Pronouns: ʃi:
- 🌐 Visit my [blog](https://sytranvn.dev/posts)
- 🌱 I’m currently learning V8, and also ML, and flute
- 🔭 I’m currently working on React SPA
<!--
**sytranvn/sytranvn** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- ⚡ Fun fact: ...
-->
## I know a little bit of
![Linux](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=linux&label=&message=Linux)
![JS](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=javascript&label=&message=Javascript)
![Python](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=python&label=&message=Python)
![Git](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=git&label=&message=Git)
![Bash](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=gnu-bash&label=&message=Bash)
![AWS](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=amazon-aws&label=&message=AWS)

and a little bit of  
![C++](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=c&label=&message=C%2FC%2B%2B)
![Go](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=go&label=&message=Go)
![Java](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=java&label=&message=Java)
![Octave](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=octave&label=&message=Octave)
![Docker](https://img.shields.io/static/v1?style=square&color=0F0F0F&logoColor=FFFFCC&logo=docker&label=&message=Docker)

## I pushed a few lines of code to
- [react](https://github.com/facebook/react)
    - [4e5d7fa](https://github.com/facebook/react/commit/4e5d7faf54b38ebfc7a2dcadbd09a25d6f330ac0)
- [ssh-chat](https://github.com/shazow/ssh-chat)
- [owncast-admin](https://github.com/owncast/owncast-admin)
    - [2e6456c](https://github.com/owncast/owncast-admin/commit/2e6456c1c02ee8ed49ec6f31039dfede86c6e447)
- [chrome-extension-cli](https://github.com/dutiyesh/chrome-extension-cli)
    - [e2df8d5](https://github.com/dutiyesh/chrome-extension-cli/commit/e2df8d5d0541a9815a1ccd8554d5fad0e373389f)

## Oh my .rcs
### .zshrc
<details>
  <summary>Click to expand!</summary>
    
```shell
export EDITOR='vim'                                                                
                                                                                   
setopt HIST_IGNORE_ALL_DUPS                                                        
setopt HIST_IGNORE_SPACE                                                           
                                                                                   
RPROMPT='$(date +%T)'                                                              
eval "$(/opt/homebrew/bin/brew shellenv)"                                          
                                                                                   
export NVM_DIR="$HOME/.nvm"                                                        
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm                  
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
                                                                                   
eval "$(direnv hook zsh)"                                                          
if [ -f ~/.git-prompt.sh ]; then                                                   
    source ~/.git-prompt.sh                                                        
    export GIT_PS1_SHOWDIRTYSTATE=true                                             
    export GIT_PS1_SHOWUNTRACKEDFILES=true                                         
    export GIT_PS1_SHOWUPSTREAM="auto"                                             
    PROMPT='%{$fg[red]%}%m%{$reset_color%}:%{$fg[green]%}%c%{$reset_color%}$(__git_ps1) %(!.#.$) '
fi                                                                                 
# aliases                                                                          
alias zrc='vim ~/.zshrc'                                                           
alias zrl='source ~/.zshrc'                                                        
alias ll='ls -lahG'                                                                
                                                                                   
path+=(~/.bin)      
```
    
</details>

### .vimrc
<details>
  <summary>Click to expand!</summary>  

```vim
set nocompatible          " get rid of Vi compatibility mode. SET FIRST!        
filetype plugin indent on " filetype detection[ON] plugin[ON] indent[ON]        
set t_Co=256              " enable 256-color mode.                              
syntax enable             " enable syntax highlighting (previously syntax on).  
colorscheme desert        " set colorscheme                                     
set number                " show line numbers                                   
set laststatus=2          " last window always has a statusline                 
filetype indent on        " activates indenting for files                       
set nohlsearch            " Don't continue to highlight searched phrases.       
set incsearch             " But do highlight as you type your search.           
set ignorecase            " Make searches case-insensitive.                     
set ruler                 " Always show info along bottom.                         
set autoindent            " auto-indent 
set softtabstop=4         " unify                                                  
set shiftwidth=4          " indent/outdent by 4 columns                            
set shiftround            " always indent/outdent to the nearest tabstop           
set expandtab             " use spaces instead of tabs                             
set smarttab              " use tabs at the start of a line, spaces elsewhere   
autocmd Filetype javascript setlocal ts=2 sw=2 sts=0 expandtab                     
set nowrap                " don't wrap text                                        
" make backspaces more powerfull                                                   
set backspace=indent,eol,start                                                     
                                                                                   
set showcmd             " show (partial) command in status line                    
set noswapfile                                                                     
                                                                                   
set splitright          " show split window to the right                           
                                                                                   
set nu                                                                             
                                                                                   
set list                                                                           
set listchars=tab:┆\                                                               
                                                                                   
set colorcolumn=80                                                                 
                                                                                   
call plug#begin()                                                                  
" Multiple Plug commands can be written in a single line using | separators     
Plug 'SirVer/ultisnips' | Plug 'honza/vim-snippets'                             
                                                                                
" post install (yarn install | npm install) then load plugin only for editing supported files
Plug 'prettier/vim-prettier', {                                                 
  \ 'do': 'yarn install --frozen-lockfile --production',                        
  \ 'for': ['javascript', 'typescript', 'css', 'less', 'scss', 'json', 'graphql', 'markdown', 'vue', 'svelte', 'yaml', 'html'] }
                                                                                
Plug 'ludovicchabant/vim-gutentags'                                             
                                                                                
call plug#end()   
```
   
</details>
