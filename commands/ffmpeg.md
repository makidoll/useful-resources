# Trim a video 

`ffmpeg -i movie.mp4 -ss 00:00:03 -t 00:00:08 -async 1 -c copy cut.mp4`

# Images to video

```
ffmpeg -r 30 -i %04d.png -c:v libx264 -pix_fmt yuv420p -preset veryslow -crf 23 out.mp4
ffmpeg -r 30 -i %04d.png -c:v libx264 -preset veryslow -crf 23 out.mkv
```

# Replace audio in video

`ffmpeg -i v.mp4 -i a.wav -c:v copy -map 0:v:0 -map 1:a:0 new.mp4`
