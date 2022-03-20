# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **ROLLAND MUZEYA**

Time spent: **4** hours spent in total

Link to project: (https://glitch.com/edit/#!/acoustic-marshy-limpet)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://user-images.githubusercontent.com/76987595/157788343-39af9d37-8c6c-44f2-92ba-f591fef8c318.gif)
![](gif2-link-here)
![](gif3-link-here)
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

https://www.the-art-of-web.com/javascript/creating-sounds/

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

I encountered a challenge in trying to understand all the Javascript  sound synthesis functions using the AudioContext library. After reading through the functions that I had to copy and paste into my “scripy.js” file, I had no idea how or why we had to include all the method calls we used to generate the tones. I had a tough time understanding the relevance of method calls like the createOscillator() and createGain() in producing tones. However, after close study of the AudioContext library, I understood that the OscillatorNode referred to the wave type, and the gainNode was simply the change in volume of the sound. Despite the complexity of the code in the SoundPlayer class, I realized that my understanding of key terms of the AudioContext interface was enough for me to understand how code in the sound synthesis functions was serving to produce the tones whenever a button was clicked. Moreover, playing around with the numbers in the freqMap object helped me become more comfortable using the library. Finally, playing around with the values in the pattern array allowed me to have control over the sequence of clues that was to be played, and this consolidated my understanding of the playCueSequence() function.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

To start with, if we were to build a more complex web application that would incorporate the use of a backend and database, besides considering the loading time for a webpage and security features in a programming language, are there other factors to be considered when choosing which language to use for the application? Also, is there need for one to have extensive knowledge of networking and cybersecurity when building web applications? Finally, is there a need for a developer to have in-depth knowledge of the implementation of libraries used in an application, or it is adequate to only know how to invoke and use methods from libraries?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

To begin with, I would implement a feature that keeps a record of player's scores on a scoreboard even after exiting the game. In addition, I would include a feature that allows a player to choose a difficulty level. A hard difficulty level being one where the clue sequence is played at a fast rate. Moreover, I would include a “special” mode where the player can choose to play until they fail. I would dynamically grow the size of the pattern array on each turn with randomly generated numbers within the range of the number of buttons available. As long as the player guesses correctly, a randomly generated number is added to the pattern array, and its corresponding tone is added to the clue sequence.

## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.loom.com/share/f8703e726dc74635944fd2f5474854e9)


## License

    Copyright [YOUR NAME]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

