# gif cheatsheet

## Magick

Installation

```bash
brew install imagemagick
```

Image sequences to GIF

```bash
convert *.png(n) out.gif
convert $(ls *.png | sort -V) out.gif
convert -delay 50 *.png out.gif
```

### GIF loop

Infinite loop

```bash
convert -loop 0 ani.gif ani.gif
```

Finite loop

```bash
convert -loop 1 ani.gif ani.gif
```
