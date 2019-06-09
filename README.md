## Visual Music WebApp
An app that converts your favorite music pieces into visual expressions. 

Visual Music is a collaboration project managed by a group of dedicated fellow students. Aimed at all music and arts lovers, it provides the users with a real time visual transcription of a streamed music piece. 

If the visual transcription can be at first of random assignment of colors and shapes, it shouldn't remain so, as **one of the main interest is to transcribe the emotional effects of the music piece**. Therefore, questions will araise as perception is highly cultural and language induced. It might be interesting in a second time to create various themes based on those considerations for the visual transcription.

## Applications
The applications could be :
* the possibility to screen the visual expression as background for parties, concerts and stages, 
* accessibility, by giving a visual transcription of music pieces, making them accessible to the hearing impaired,
* creation of original objects, with the possibility of a screen capture going with a downloadable HD print file, the possibility of printing, framing and offering the painting of a song to friends and family,
* tool or interesting experiment for musicologists, linguists, scientists, etc.

## Technology/Stack:
Is being defined.  

* React and Redux
* CSS3 Flexbox & Grid System
* Javascript
* P5 ?
* Soundcloud
* Figma to design the UI interface?

Potential Add-On:
* [StoryBook](https://storybook.js.org/) Will let us test components individually

__Idea:__ Stream Soundcloud music, take the data that we have and process it through p5.js. 

The readme of that project [soundcloud-visualizer](https://github.com/michaelbromley/soundcloud-visualizer) is a good explanation: Soundcloud sends 2 variables, that can be parsed to create a visualization based on those.

__Examples of Soundcloud implementations:__            
https://codepen.io/DonKarlssonSan/pen/bdNBMz                
https://www.reddit.com/r/visualization/comments/54lxof/soundcloud_music_visualizer/        

### Challenges to solve to define tech/stack
#### Data limit of server if uploading MP3: 
> justinwlin: 
> The main problem I think with this project is how to upload MP3 and process it. If we allow people to just upload mp3s, and add it to some asset folder, will it just forever buildup in our assets folder taking up space and eventually crashing the server when we exceed the memory limit?

> Or if someone uploads a particularly large mp3 and blows through the data limit of a server, or if there are multiple people uploading files, etc, how do we handle that? 

* https://www.npmjs.com/package/localforage ?                 

#### Browser implementation of HTML5 APIs
HTML5 provides interesting APIs that could do the job for the project, but there might be browser implementation issues, it seems to work best with Chrome, and we wish that our app can be accessed from most modern browser as possible :                
* HTML5 File System API: https://code.tutsplus.com/tutorials/toying-with-the-html5-file-system-api--net-24719              
* HTML5 Web Audio API: https://www.html5rocks.com/en/tutorials/webaudio/intro/            
* https://www.html5rocks.com/en/tutorials/getusermedia/intro/               
* https://caniuse.com/#search=web%20audio%20api               
* https://www.youtube.com/watch?v=xmGv_Schm5U                          

This is the solution chosen in Preziotte Party Mode: https://github.com/preziotte/party-mode
along with d3.js: https://d3js.org/

#### Streaming the audio with SoundCloud API:
Again, browser issues are reported in the https://github.com/michaelbromley/soundcloud-visualizer README:
> Since the web audio API is pretty new, browser support is patchy:
> * Chrome Latest versions works well, that's what I've been building in.
> * Firefox This should work, since it has supported web audio since version 25, but in my tests the audio fails to play. Any suggestions?
> * Safari I haven't tested it since I'm stuck with the dead Windows version, but I guess it should work since it's WebKit.
> * IE Nope.
> * Opera Not tested but maybe now that they switched to WebKit.

## Useful Links
[Zero to Mastery - Guidelines on open source](https://github.com/zero-to-mastery/start-here-guidelines)            
[CONTRIBUTING.md](https://github.com/zero-to-mastery/visual-music/blob/master/CONTRIBUTING.md)


## Functionalities
### Version 1.0
* 2 pages:
  * landing page
  * player page
* Soundcloud streaming
* Play/Stand-By
* Export and download screen capture
* One main theme for visual transcribe
* No registration
    
### Version 2.0
* New visual themes
    
### Version 3.0
* (User can upload audio files?)
* (User can input live music?)

## Release & Launch
Visual Music is being built with the intention of releasing and maintaining the project in the real world. Therefore providing contributors with a great opportunity to expand on and learn new skills, being part of a project that can be included on resumes and showed off to friends, family and potential employers.

Should be discussed and decided by the team in charge when constituted...
* ZTM Discord
* LinkedIn
* ...
