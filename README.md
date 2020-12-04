# web-path
https://zfaka.github.io/web-path/
Accenture
Despegar
Epidata
Avalith
Ayi & Asociados
Baufest
Belatrix Software
BVS Technology Solutions Technology
Capgemini
Data IQ
Edrans
Everis
EY
Flux IT
Global Hitss
Globant
Indra
intive
Itrio SA
Mercado Libre
NEORIS
Practia Global
PwC Argentina
QActions
Quadion Technologies
Sofrecom
Softtek
Capgemini
Intive
TSoft
Baufest
Softtek
Proyecto Nahual
Summa Solutions
TATA Consulting Services
Tsoft
Émerix
Xappia
valkimia
Xperis
Coder.io
GlobalLogic
DXC Technology






























syntax on

set pastetoggle=<F3>
set nu
set noswapfile
set nobackup
set autoindent
set smartindent
set smartcase
set tabstop=4 
set softtabstop=4
set shiftwidth=4
set expandtab
set nowrap
set undodir=~/.vim/undodir
set undofile
set incsearch
set colorcolumn=80
set rnu

set runtimepath^=~/.vim/bundle/ctrlp.vim

call plug#begin('~/.vim/plugged')
Plug 'neoclide/coc.nvim', {'branch': 'release'}
Plug 'tweekmonster/gofmt.vim'
Plug 'tpope/vim-fugitive'
Plug 'vim-utils/vim-man'
Plug 'sheerun/vim-polyglot'
"Plug 'junegunn/fzf', { 'do': { -> fzf#install() } }
"Plug 'junegunn/fzf.vim'
"Plug 'tpope/vim-dispatch'
Plug 'sainnhe/gruvbox-material'
Plug 'vim-airline/vim-airline'
Plug 'Valloric/YouCompleteMe'
Plug 'mattn/emmet-vim'
Plug 'preservim/nerdtree'
Plug 'vuciv/vim-bujo'
call plug#end()
"salir del modo insert "
inoremap jj <ESC>
"hotkey to open Todo Bujo"
map <C-x> :Todo<CR>
"size de vim Bullet Journall Bujo
let g:bujo#window_width = 50

"Close nerdtree after open a file
let g:NERDTreeQuitOnOpen = 1
"Show hidden files
let NERDTreeShowHidden=1
"Hotkey to open NERDTree
map <C-n> :NERDTreeToggle<CR>

"Automatically closing braces
inoremap { {<CR>}<Esc>ko<tab>
inoremap [ [<CR>]<Esc>ko<tab>
inoremap ( (<CR>)<Esc>ko<tab>

"Normal brackets
inoremap ) ()<Esc>i
inoremap ] []<Esc>i
inoremap } {}<Esc>i

"Automatically close comillas
inoremap ` ``<Esc>i
inoremap ' ''<Esc>i
inoremap " ""<Esc>i

"make a space after comma"
inoremap , ,<Space>
" Important!!
if has('termguicolors')
    set termguicolors
endif

let s:background_color="NONE"
" For dark version.
"set background=dark

" For light version.
"set background=light

" Set contrast.
" This configuration option should be placed before `colorscheme gruvbox-material`.
" Available values: 'hard', 'medium'(default), 'soft'
"let g:gruvbox_material_background = 'soft'

""colorscheme gruvbox-material
let g:airline_theme = 'gruvbox_material'

map <C-m> gg=G<C-o><C-o>
