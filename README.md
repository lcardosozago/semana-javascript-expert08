# JSExpertHub Pre-processing videos in browsers - JS Expert Week 8.0

## This project is experimental and aims to preprocess videos in the client's browser in order to save resources.

Welcome to the eighth Javascript Expert Week. This is the starter code to begin our journey.

Star this project with a 🌟 and join our [official WhatsApp group](https://l.erickwendel.com.br/jse8-grupo)

## Preview
<img width=100% src="./initial-template/demo.gif">

## Pre-requirements
- This project was created using Node.js v18.17.0
- It's recommended that you run the project in a Unix environment (Linux). If you are on Windows, it's advised to use [Windows Subsystem for Linux](https://www.omgubuntu.co.uk/how-to-install-wsl2-on-windows-10) because the lessons showcase Linux commands that might not exist on Windows.

## Important
- Every day at 6 pm I'm uploading the day's lesson code in [classes](./classes). If you are starting the project, remove the [classes](./classes) folder to start from scratch!

## Running
- Run `npm ci` in the folder containing the `package.json` file to restore packages.
- Execute `npm start` and then go to your browser at [http://localhost:3000](http://localhost:3000) to view the page above.

## Checklist Features

- Video Uploader
  - [] - Should understand MP4 format videos even if they are not fragmented.
  - [] - Should process items in isolated threads with Web Workers.
  - [] - Should convert video fragments to `144p` format.
  - [] - Should render frames in real-time on a canvas element.
  - [] - Should generate WebM files from fragments.

### Challenges
- [] - Encode in 360p and 720p.
- [] - Do audio track encoding/decoding.
- [] - Also upload the audio track.
- [] - Concatenate the final file on the server into a single file.
- [] - Fix the Webm issue of not displaying video duration.
- [] - Fix the website's responsiveness.
- [] - Try using other muxers.
  - https://github.com/Vanilagy/webm-muxer
  - https://github.com/Vanilagy/mp4-muxer

### Links shown in the lessons:
- I've gathered all the links in [references](./referencias.md).

### Notes
- Ask your questions about the challenges in our community; the goal is for you to learn in a fun way. Any doubts? Ask there!

- Upon completing any of the challenges, post in the **#desafios** channel of the community on **Discord**.

### FAQ
- browser-sync is throwing errors on Windows and never starts:
  - Solution: Replace browser-sync with http-server.
    1. Install **http-server** with `npm i -D http-server`.
    2. In package.json, delete the entire `browser-sync` command and replace it with `npx http-server .`.
    3. Now the project will run on :8080, so go to your browser and try accessing http://localhost:8080/
  The only thing is that the project won't restart when you change some code; you'll need to refresh the page every time you make a change.
