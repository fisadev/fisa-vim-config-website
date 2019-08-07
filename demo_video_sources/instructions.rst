To generate the demo video, export the video in the selected 1280x720 profile, and then crop it with ffmpeg:
ffmpeg -i demo_video_sources/demo_raw.mp4 -filter:v "crop=985:573:148:80" videos/demo.mp4

To generate the feature videos, convert them with:
ffmpeg -i demo_video_sources/x.mp4  -filter:v "crop=950:553:52:80" videos/features_x.mp4
