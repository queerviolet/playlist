# What this does

It's designed as a video queueing system for events where you
have a bunch of people presenting, each with their own screencast.

It starts off showing the Grace Hopper / Fullstack logo.

When you hit *space*, it plays the first video.

When that video is done, it shows the logo again.

When you hit *space* again, it plays the next video.

When it's done, the logo appears again.

Etc.

# Keyboard shortcuts

**Space:** Play / Pause
**⌥ right:** Next video
**⌥ left:** Previous video
**⌥ right:** Next video
**⌥ left:** Previous video
**^⌘ left:** Seek back 15 seconds
**^⌘ right:** Seek forward 15 seconds

# How to use this

First, clone this repo.

You'll see that `index.html` has a bunch of `<video>` tags:

html```
    <video src="1609/pgb-vsu.mp4" data-volume=1></video>
    <video src="1609/GH - Pioneers of Mars.mp4"></video>
    <video src="1609/GH - paraGraphic.mp4"></video>
```

Put the paths of your videos in there.

Videos are *muted* by default. If you don't want a particular video
to be muted, you can specify the `data-volume` attribute (a float,
clamped 0.0 to 1.0) to turn it up for that video only.

Then open the file in Chrome.