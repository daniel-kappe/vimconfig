# NeoVIM Configuration

## Installation

(Optional|use init.vim.without-coc) coc code completion requires nodejs:

```sh
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Download vim-plug:

```sh
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

Link _init.vim_ in _~/.config/nvim_:

```sh
ln -s init.vim ~/.config/nvim/init.vim
ln -s init.vim ~/.config/nvim/init.vim.without-coc
```

Install the Plugins:

```sh
nvim -c "PlugInstall|q|q"
```

## Setup Code Completion

Run CocInstall with selected languages

```sh
nvim -c 'CocInstall <language1> <language2> ...|q|q'
```

Choices are:

- coc-json
- coc-html
- coc-css
- coc-prettier
- coc-python
- coc-markdownlint
- coc-svg
- coc-xml
- coc-yaml
