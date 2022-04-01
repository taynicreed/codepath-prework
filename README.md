# Pre-work - *Memory Game*

Rainbow Memory Game is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Taylor-Nicole Reed

Time spent: 5 hours spent in total

Link to project: (https://glitch.com/edit/#!/rainbow-memory-game) 


## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn


## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](http://g.recordit.co/A96JvXZQSR.gif)
![](http://g.recordit.co/v3RnjprZgv.gif)
![](http://g.recordit.co/lXDsqYnF7j.gif)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 

I used information learned in a course at Oregon State University, taught by Nauman Chaudhry and Pam Van Londen.
Additional websites referenced: 
https://cssreference.io/
https://www.w3schools.com/css/
https://coolors.co/


2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? 

After I finished all of the required components and was testing my game, I realied that the buttons were not changing colors as expected. The code was running without any errors, so I knew that this was not a syntax problem and I had made a mistake somewhere with my code logic. 
My first step in trying to correct this was to do some tests to recreate the problem and understand exactly when it was occurring. I discovered that the buttons behaved correctly when manually clicked by the player, but when they were played as part of the clue sequence they would change to the "lit" color and would not go back to the default color until the page was refreshed.
Due to this I was able to conclude that there was an issue with my clearButton function. I closely reviewed this function and compared it with the lightButton function to figure out the problem. I had written both functions to: classList.add("lit"). Once I changed the clearButton function to classList.remove("lit"), the game ran as expected. 

3. What questions about web development do you have after completing your submission?

What do I make sure my product is accessible? How can I make sure my web pages are easy to navigate with a screen reader, readable in different contrast modes, display correctly if magnified, etc. 
What are best practices when designing websites that may be viewed through many different browsers and devices? 
How can I use CSS to make my projects look better? 
How do I take the code I write and make it into a website? 

4. If you had a few more hours to work on this project, what would you spend them doing? 

I would spend more time learning about CSS so I could add more personalization to my project and make it look nicer.

I would also like to add settings that the player can adjust to make the game easier or harder: 
- Clue speed (slow, normal, fast)
- Difficulty level (3 strikes, 2 strikes, 1 strike)
- Number of clues (8, 16, 24)
- Timed or untimed

I think having options like this would increase the "replayability" factor of the game, as the player could start with the easiest level and work up to harder levels. 


## Interview Recording URL Link

[My 5-minute Interview Recording](https://youtu.be/pyivpFWesFs)


## License

    Copyright Taylor-Nicole Reed

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
    
    
