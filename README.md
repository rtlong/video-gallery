This is video-gallery. It's a simple bash script to facilitate the generation of those thumbnail 
overviews you've probably seen before:

![Sample output](/rtlong/video-gallery/raw/master/example.png)

# Why?

I wrote it because I needed a way to preview a video's content without opening the actual video.

# Usage

Couldn't be easier: 

```
$ video-gallery VIDEO_FILE
```
It will save the image as a PNG in the same directory as the video, with the same name.

Currently, it only accepts one file at a time, but that's easy to deal with using a for loop:

```
$ for vid in {video1,video2,etc}; do video-gallery "$vid"; done
```

It shouldn't be hard to customise to your liking. I've included most of the major options at the 
top of the file.

# Todo

I intend to add support for many different options on the command line, including support for 
providing the script with multiple videos.

# Thanks

I must acknowledge the efforts of:

- [Rupert Plumridge](http://www.prupert.co.uk/2011/04/07/a-better-ffmpeg-progress-script/)
- [Rich Jerrido](http://www.outsidaz.org/blog/2009/10/26/screencap-generation-via-ffmpeg-and-imagemagick/)

...for the bits of their that code I used, which is noted in the script.
