<img src="http://rawgit.com/caiogondim/maglev/master/logo/logo.svg">

# Maglev (forked for base16-oceanicnext)

[See original](https://github.com/caiogondim/maglev)

## Screenshot

<img src="http://rawgit.com/sohkai/maglev/master/img/screenshot.png">

## Installing

This plugin depends on the following tmux plugins:

- [Tmux Pain Control](https://github.com/tmux-plugins/tmux-pain-control)
- [Tmux copycat](https://github.com/tmux-plugins/tmux-copycat)
- [Tmux Yank](https://github.com/tmux-plugins/tmux-yank)
- [Tmux Open](https://github.com/tmux-plugins/tmux-open)
- [Tmux Battery](https://github.com/tmux-plugins/tmux-battery)
- [Tmux CPU](https://github.com/tmux-plugins/tmux-cpu)

See [installing TPM plugins](https://github.com/tmux-plugins/tpm#installing-plugins).

You will have to declare the plugins and the theme on your `.tmux.conf`:

```bash
# Start windows and panes at 1, not 0
set -g base-index 1
set -g pane-base-index 1

set-option -g status-position top

set-option -g repeat-time 0

# Removes ESC delay
set -sg escape-time 0

# List of plugins
set -g @tpm_plugins '                     \
    caiogondim/maglev                     \
    tmux-plugins/tpm                      \
    tmux-plugins/tmux-sensible            \
    tmux-plugins/tmux-resurrect           \
    tmux-plugins/tmux-continuum           \
    tmux-plugins/tmux-yank                \
    tmux-plugins/tmux-pain-control        \
    tmux-plugins/tmux-copycat             \
    tmux-plugins/tmux-open                \
    tmux-plugins/tmux-battery             \
    tmux-plugins/tmux-cpu                 \
    tmux-plugins/tmux-prefix-highlight    \
'

# Initialize TMUX plugin manager
run '~/.tmux/plugins/tpm/tpm'
```

This Tmux theme was made to work with [Bullet train](https://github.com/caiogondim/bullet-train-oh-my-zsh-theme) ZSH theme.

Some dependencies:
- [Tmux](http://tmux.github.io/)
- [TPM](https://github.com/tmux-plugins/tpm)
- [Powerline patched font](https://github.com/powerline/fonts)

## Credits
- [Original](https://github.com/caiogondim/maglev)
