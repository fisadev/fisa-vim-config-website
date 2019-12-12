Capture the whole thing in one go, using a white background below the terminal app.

Then use openshot to crop the parts of the video, and add the titles.

Finally, crop the black borders with something like this:
ffmpeg -i demo_video_sources/demo_raw.mp4 -filter:v "crop=985:573:148:80" videos/demo.mp4 
Where the crop parameters are "out_w:out_h:x:y"
- out_w is the width of the output rectangle
- out_h is the height of the output rectangle
- x and y specify the top left corner of the output rectangle
