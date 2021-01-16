# vim-pack

new machine operations
```
cd .vim
git clone git@github.com:raymatthes/vim-pack.git pack --recursive
```


local operations to add a plugin
```
git submodule add https://github.com/altercation/vim-colors-solarized colors/start/vim-colors-solarized

git submodule add https://github.com/vim-airline/vim-airline plugins/start/vim-airline

git add -A
git commit "added plugin"
git push
```


https://medium.com/@paulodiovani/installing-vim-8-plugins-with-the-native-pack-system-39b71c351fea
```
# make the pack folder a git repository
cd ~/.vim/pack
git init

# add as many plugins as you want in the desired
# package directories

# add vim-airline as autoloaded in plugins/ directory
git submodule add https://github.com/vim-airline/vim-airline plugins/start/vim-airline

# add the one color scheme in the colors/ directory
git submodule add https://github.com/altercation/vim-colors-solarized colors/start/vim-colors-solarized

# and optinaly, we want the elixir syntax and compiler tools under syntax/
git submodule add https://github.com/elixir-lang/vim-elixir syntax/opt/elixir

# start vim and configure the plugins as desired :)
cd -
vim ~/.vimrc

# when need to update,
# it is just a matter of updating submodules
git submodule update --remote --merge
git commit
```

