# Stretch & Fold Tracker - CS50 Final Project
#### Video Demo:  <URL HERE>
#### Description:

As my final project for CS50 course, I wanted to create something that I knew I would benefit myself from. I have been baking sourdough bread for a few months now, but one thing has been bothering me ever since I started: keeping track of the stretches and folds. In order for the dough to develop gluten and turn into a soft, bouncy loaf of bread, it is recommended to stretch it a few times, every 30-45 minutes. Unfortunately, I would often forget which set of stretches I am on, or even accidentally ignore the timers I have set on my phone. Eventually, I started using my smart watch and a notepad, but I thought that a simple, aesthetically pleasing online tool could help not only myself, but others who have busy lives, as well.

I wanted to keep the user interface minimalistic and intuitive, but also bright and playful. Therefore, I chose a simple combination of HTML + CSS + JavaScript as my tools and GitHub Pages as my hosting. My plan was to launch the MVP as soon as possible and test it out with a real audience - people who bake sourdough regularly - in order to gather some feedback and suggestions for features. The first iteration of the tool was just two elements and two buttons: a stretch & fold **counter**, a **timer set for 30 minutes**, a **button to reset the tracker**, and a **button** to increment that counter and **restrat the 30 minute timer**. I also had a notification sound implemented that played once the timer reached 00:00.

![Opera Snapshot_2024-09-04_130357_korniann github io](https://github.com/user-attachments/assets/76b86d1c-5fc9-4906-b238-3100127342a0)

After making sure that the basic functionality is there, I chose a color palette and used CSS to implement it.

![Opera Snapshot_2024-09-05_110857_korniann github io](https://github.com/user-attachments/assets/ba5946e2-d9b8-4682-b54e-ab7414c8ab4e)

Following my plan to test it out with a real audience, I published the tracker on GitHub Pages and posted it in a couple of places on social media. The responses were mixed: some people did not understand the need for a tool like this when phone timers and paper exist, others praised the idea, and some asked about different features that they would like to see in a tool like this. I have saved all of the responses and chose to work on a couple of suggestions that were mentioned the most: the ability to change the time between the stretches (instead of it being set at 30 min), and the ability to track the stretches for multiple loaves at a time. 

I started by editing the original JavaScript for the timer itself and wrote a few more lines of code that allows the user to input their desired amount of time between the stretches. I then created a function to toggle the visibility of the time input element - I needed it to appear as soon as the page loads and then hide once the timer has been set, allowing the timer itself to appear.

![Opera Snapshot_2024-10-21_154533_korniann github io](https://github.com/user-attachments/assets/ee387404-8a30-49f4-8149-a63af8088988)

For the feature to track multiple loaves of bread at the same time, I first needed to code a way to differentiate between the different timers and trackers, so I wrote a script that assigns and increments a unique tracker ID for each of the new trackers created, and identifying the first tracker that loads as "Default Tracker". From there, I used Bootstrap as my starting point to create a tab-based navigation interface, which I then modified using custom CSS. I wrote a new script that allows the user to rename their tracker at any point in time, which also updates the name of it in the tab navigation. My JavaScript now assigns a new tracker ID when the "Add New" tab is clicked, and generates a new set of elements with that that ID using a template. All of the original scripts also had to be adjusted in order for them to be able to differentiate between the unique trackers and timers.

![Opera Snapshot_2024-11-01_150119_korniann github io](https://github.com/user-attachments/assets/0eb8f73d-e85a-4736-a089-32ac42e04c49)

As I was testing the tool throughout the whole process, I found many things that I either broke by writing new code, or did not function/ look the way I wanted. But one of them was particularly interesting to me - I've noticed that the notification sound was not playing when multiple timers reached 00:00 at around the same time. I learned that a new sound will not start playing if there's another one still playing, so I had to modify my script to pause the sound, reset it to the beginning, and play it again, as soon as another timer hit 00:00. 

This is where the project stands as of this point, November 2024. I plan on continuing working on it in the foreseeable future, and you can see my plans below. Thank you for reading!

---
Tentative to do:

[x] delete the css and start over/ clean it up and organize better

[x] remove the navbar

[x] style up the privacy policy a bit

[x] decide on the color palette

[x] find 2 matching fonts

[x] create a design

[x] implement the new design in css

[x] optimize the responsiveness - fix the box width wtf

[x] finish setting up ko-fi and add it to the website

[ ] spice up the interface (the timer)

[x] add a way to set a custom timer

[ ] add a first fermentation feature?

[ ] add a bulk fermentation feature?

[ ] optimize the SEO?

[x] buttons/ navigation for multiple loaves

[x] the ability to name the timers/ loaves

[ ] database

[ ] sign up + login

[ ] journal

[ ] logging temperature 




