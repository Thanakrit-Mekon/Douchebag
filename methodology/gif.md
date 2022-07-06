# gif cheatsheet

## Magick

#### Installation

```
brew install imagemagick
```

#### Image sequences to GIF

```
convert *.png(n) out.gif
convert $(ls *.png | sort -V) out.gif
convert -delay 50 *.png out.gif
```

#### GIF loop

Infinite loop

```
convert -loop 0 ani.gif ani.gif
```

Finite loop

```
convert -loop 1 ani.gif ani.gif
```
