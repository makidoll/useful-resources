# ImageMagick

PNG files to GIF

```
convert -loop 0 -delay 100/60 *.png out.gif
convert -loop 0 -delay 100/60 *.png -interpolate Nearest -filter point -resize 400% out.gif
```
