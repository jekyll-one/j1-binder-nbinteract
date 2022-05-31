# J1 NBI Binder Repo

Configuration settings and all notebooks used by the J1 NBI Integration.

## apt.txt

Added ffmeg to make it usable for e.g matplotlib animations

### NB config

#### matplotlib animation

The method (of the animation instances) to manage the
player is controlled by the animation rc parameter.

The rc parameter currently supports values of "none", "html5"
and "jshtml".

*  none:    no player (display) is shown    
*  html5:   use the native HTML5 player widget
*  jshtml:  use the interactive JavaScript widget

The default is none to not display a player. To display
the native HTML5 player, # set it to "html5". For the
interactive JavaScript widget to "jshtml".

```
rc('animation', html='html5', embed_limit='256')
# rc('animation', html='jshtml', embed_limit='512')
```

**NOTE**: The JavaScript widgets referenced to **jshtml** does currently
**not** work.
