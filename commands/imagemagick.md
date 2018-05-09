# ImageMagick

PNG files to GIF

```
convert -loop 0 -delay 100/60 -alpha set -dispose previous *.png out.gif
convert -loop 0 -delay 100/60 *.png -interpolate Nearest -filter point -resize 400% out.gif
```

GIF to PNG

```
convert -coalesce in.gif %04d.png
```

PNG files to spritesheet

```
montage *.png -background none -geometry +0+0 -tile x1 out.png
```
