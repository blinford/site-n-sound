# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Benjamin Linford

Time spent: 1.5 hours spent in total

Link to project: https://glitch.com/edit/#!/site-n-sound

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

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [x] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [x] Included an HTML representation for the timer

## Video Walkthrough

Here's a walkthrough of implemented user stories:
https://cdn.glitch.com/c843f282-85fe-456e-9ffb-33d1a9b974a3%2Fezgif-7-478099733423.gif?v=1616634281725

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

www.w3schools.com/jsref

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

When I was coding the timer, I found it difficult to keep track of the different threads that the program was running. For example, I used two different timers to implement the countdown. One of the timers controlled the HTML representation ("x seconds left"), and the other timer kept control of the overall countdown. Although I considered condensing the two timers into one singular one, I found that it was easy to handle both of them at the same time. When I reset the HTML representation, I should also reset the countdown in the background. To group these timers together, I included a function that would reset all the necessary components of the timer. This made it super easy to conceptualize when I needed to reset the timer, since I could do a full reset when the user either makes a guess or runs out of time.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

The project was interesting to complete, but it made me wonder about the portability of the application. The "flow" layout of the HTML elements allowed for some variability in screen size, but there certainly must be some limitations. If the screen were too thin, it could prevent the game from being played properly. However, I think it might be ever more to consider the "comfort" of the user. Sometimes when I am on a companies website, the phone's limited screen size throws the entire layout into disarray. There can be overlapping elements and hidden objects which makes those websites super difficult to navigate. I would like to learn more about how the HTML/css/js combo can be used to account for this variability and make websites more user friendly. I also wonder how programmers manage all of these simultaneous threads and timeout functions. It was difficult to keep track of during coding.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

When I play similar pattern-following games, I find myself relying on the spatial layout of the elements a lot. I usually remember some sequence of directions like "top-right, down, left" rather than "blue, yellow, red." I just found about this internship a few hours ago (the day it is due), so I'm certainly pressed for time, but I think it would be a great challenge to reorder the squares each time there is a successful guess. The biggest obstacle I see in changing that is reordering the representations of buttons in the HTML document. I looked into reorganizing HTML elements, and some sources mentioned that I could rewrite the html, but I wasn't sure if that would be the best option. 



## License

    Copyright Benjamin Linford

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.