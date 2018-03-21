# Trim a video 

`ffmpeg -i movie.mp4 -ss 00:00:03 -t 00:00:08 -async 1 -c copy cut.mp4`

# Images to mp4

`ffmpeg -r 60 -i %04d.png -c:v libx264 -vf "fps=60,format=yuv420p" out.mp4`