To generate the demo video, export the video in the selected 1280x720 profile, and then crop it with ffmpeg:
ffmpeg -i demo_raw.mp4 -filter:v "crop=985:573:148:80" demo.mp4

To generate the feature videos, convert them with:
ffmpeg -i x.mp4 -filter:v "crop=985:573:48:80" feature_x.mp4
