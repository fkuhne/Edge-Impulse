# Environment Sounds

This project uses an Arduino Nano 33 BLE Sense to listen to sounds out there.

Currently, supports two sounds:
* rain (turns the blue led on)
* noise (turns the red led on)

## Dataset

It has some samples of rain noise recorded with my smartphone and sliced with Audacity.

## Edge Impulse project

* https://studio.edgeimpulse.com/public/33605/latest

## Some useful commands

* Transforms a list of wav files to 16000 Hz sampling:
```
find *.wav -print | xargs -n 1 | xargs -I {} ffmpeg -i {} -ar 16000 {} -y
``` 

* Transforms from stereo sound to mono:
```
find *.wav -print | xargs -n 1 | xargs -I {} ffmpeg -i {} -ac 1 {} -y
```

* For each wav audio file, cut it to 1 second:
```
find *.wav -print | xargs -n 1 | xargs -I {} ffmpeg -i {} -ss 00:00:00 -t 00:00:01 {} -y
``` 

