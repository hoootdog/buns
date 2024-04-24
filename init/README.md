# Initialize

## zsh

[prezto](https://github.com/sorin-ionescu/prezto)

1. Clone 
```
git clone --recursive https://github.com/sorin-ionescu/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"
```

2. Configuration
```
setopt EXTENDED_GLOB
for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do
  ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"
done
```

3. Set Zsh as your default shell:
```
chsh -s /bin/zsh
```

4. Use vi
```
$ vi ~/.zshrc
export EDITOR='vi'
export VISUAL='vi'
```

5. Change Theme
```
$ vi ~/.zpreztorc
zstyle ':prezto:module:prompt' theme 'pure'
```
