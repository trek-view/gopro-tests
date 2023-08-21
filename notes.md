## EXIFtool commands for creating bad tests

### Image files (jpg)

#### Change camera make to non-gopro

```
exiftool -IFD0:Make="Not GoPro" IMAGE.jpg
```

#### Change camera model to non-gopro

```
exiftool -IFD0:Model="Not GoPro" IMAGE.jpg
```

#### Add GPano stitching software

```
exiftool -XMP-GPano:StitchingSoftware="Foo" IMAGE.jpg
```

#### Add GPano projection type value

```
exiftool -XMP-GPano:ProjectionType="Bar" IMAGE.jpg
```

### Video files (360 + mp4)

#### Remove stitching software +projection type

```
exiftool -XMP-GSpherical:StitchingSoftware="" VIDEO.mp4
```

Note, this will destroy all XMP GSpherical tags, so don't need to pass projectiontype command to delete

#### Add stitching software + projection type

First install spatial-media repo

```
$ git clone https://github.com/google/spatial-media.git
$ cd spatial-media
# next line only if you use pyenv
$ pyenv local 2.X.X
$ python spatialmedia -i INPUT.MP4 OUTPUT.MP4
```