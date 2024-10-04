Capture the whole thing in one go, using a white background below the terminal app
(you can use index.html as background and SimpleScreenRecorder to select the rectangle around the terminal).
It's easier if you just launch alacritty with `alacritty -t "fisa vim config" -e fish`, to prevent tmux borders.

Then use OpenShot to trim the parts of the video and sync with the titles.

If the final compiled OpenShot video has black borders, you can crop them using ffmpeg:

`ffmpeg -i videos/demo_raw.mp4 -filter:v "crop=1920:853:0:112" videos/demo.mp4`

The format of the cropping parameters is: `width:height:x_start:y_start`.
