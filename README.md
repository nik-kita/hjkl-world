# ubuntu-hjkl
### 1.

```
sudo apt update && \
  sudo apt install xkeycaps && \
  sudo echo -e > .hjkl_on "
keycode 64 = Mode_switch

keycode 43 = h H Left H
keycode 44 = j J Down J
keycode 45 = k K Up K
keycode 46 = l L Right L
" && \
  sudo echo -e > .hjkl_off "
setxkbmap -option
"
```

### 2. now you should open "Settings" -> "Keyboard Shortcuts" and set two commands
* load alt+hjkl mode
```
xmodmap .on_hjkl
```
* unload alt+hjkl mode
```
sh .off_hjkl
```
