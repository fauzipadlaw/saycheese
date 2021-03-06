# SayCheese
Originally coded by thelinuxchoise(repository deleted).

Take webcam shots from target just sending a malicious link. Supports most unix-like OS (GNU/Linux, Android (Termux), Darwin, and FreeBSD).

<img width="1680" alt="Screen Shot 2021-07-26 at 6 32 52 AM" src="https://user-images.githubusercontent.com/15975922/126917036-8fb551c8-ee64-454b-a187-a07d67fabeac.png">


# How it works?
<p>The tool generates a malicious HTTPS page using Ngrok Port Forwarding method, and a javascript code to perform cam requests using MediaDevices.getUserMedia. </p>

<p>The MediaDevices.getUserMedia() method prompts the user for permission to use a media input which produces a MediaStream with tracks containing the requested types of media. That stream can include, for example, a video track (produced by either a hardware or virtual video source such as a camera, video recording device, screen sharing service, and so forth), an audio track (similarly, produced by a physical or virtual audio source like a microphone, A/D converter, or the like), and possibly other track types. </p>

[See more about MediaDEvices.getUserMedia() here](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia)
<p> To convince the target to grant permissions to access the cam, the page uses as default template page a javascript code made by https://github.com/wybiral that turns the favicon into a cam stream.</p>

## Legal disclaimer:

Usage of SayCheese for attacking targets without prior mutual consent is illegal. It's the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program 
## Installing:

```
git clone https://github.com/fauzipadlaw/saycheese
cd saycheese
chmod +x saycheese.sh
./saycheese.sh
```

## Tested on:
- macOS BigSur 11.5 arm64 M1
