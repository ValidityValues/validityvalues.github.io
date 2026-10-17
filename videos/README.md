# /videos — system media folder

Place MP4 or WebM videos in this folder and list them in `playlist.json`. The phone randomly interrupts itself every 20 seconds and opens a clip at **50% player volume**.

`playlist.json` supports either a simple filename:

```json
{
  "videos": ["my-video.mp4", "another-video.webm"]
}
```

Or objects with a title and optional segment start/end (seconds):

```json
{
  "videos": [
    { "src": "my-video.mp4", "title": "Unexpected system commercial", "start": 0, "end": 8.5 }
  ]
}
```

This repository includes `j5prime-chaos-reel.mp4` with three short mini-clips selected randomly by the starter playlist. For your own clips, upload the video file to this folder and edit `playlist.json`. Static GitHub Pages cannot automatically enumerate all files in a directory, so new videos must be added to the playlist.

Modern browsers may block autoplay with sound until the visitor interacts with the player. The website keeps volume at 50% and shows an enable-sound button if the browser blocks playback.
