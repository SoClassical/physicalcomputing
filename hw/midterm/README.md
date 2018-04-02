# Midterm Project

#### Project ideas: 1) Three LEDs to indicate three seconds pick number and letter, then it will tell you your fortune 2) Answer a  true/false question. A certain tune will play depending on the answer.

### The Trivia Game

#### The finished product: https://youtu.be/n2zen_ChrSQ

#### To make this, I used 2 momentary switches, one red LED, one green LED, index cards for the questions, a breadboard, and an Arduino Uno. Originally, I also had a piezo, but I scrapped that idea.

#### The concept of this game is to present 3 trivia questions with true/false choices to the audience on the index cards. If they press the correct switch, a green LED will illuminate. The incorrect answer would produce a lit up red LED. After a certain amount of time, LED would turn off and be ready for the next question.

#### The questions that will be presented are:
#### 1) The wandering albatross is the largest living bird by wingspan. (TRUE)
#### 2) Copper is the chemical element that gives the blood of lobsters their bluish tint. (FALSE- Nickel)
#### 3)  A male bee that comes from an unfertilized egg is called a drone. (TRUE)

### The process:
#### I first assembled the breadboard, which took a lot less time than I thought. Other than the supplies I listed above, I only needed 6 wires and 4 resistors. I also had a piezo on the breadboard at the time, so everything was very close together. I ended switching to a longer breadboard for more room. Because of this, I also had to find a larger box to contain my project.



#### Assembling the breadboard was no problem, but the code was a different story. When I first thought of this project idea, I did not imagine the code to be this complicated.

#### First I declared all the variables and filled in code for the setup with no problem. Fine. But that was just the beginning. Afterwards, I ran into several problems. Here are just a few:

#### https://youtu.be/Wfq76laLlAE The second switch (the false button) did not work when I pressed it, meaning no LED lit up when I pressed the switch. This was solved very easily. I had forgotten to uncomment the section in the code for the second switch.

#### https://youtu.be/BPhvuX2-ONc When I pressed a switch for an answer, the wrong LED illuminates. This means that all the answers were backwards. It seems that in my array, I had mixed up the answers.

#### https://youtu.be/gWuzvI0V5Vg Finally my code was all laid out and ready to go (or so I thought). The most problematic problem revealed itself: The LEDs did not turn off after 5 seconds like they were supposed to. No matter what I tried, I could not figure it out. In the end, I went to meet with Prof. Rodriguez in hopes of fixing this. It turned out to be an error in my logic.

#### After fixing the code, I fixed up the box (inside and out) so that it was more aesthetically pleasing--sort of. I had to make sure I could connect the Arduino to my laptop with the wire coming out of the box while also making sure the layout inside the box was clear. Inside the box are two pockets for the questions and answers.

#### If I had more time with this project, I would definitely spend more time to work out the piezo. Originally, I wanted a tune to play for a correct answer and an incorrect answer, but it was difficult for me to find time to work on the piezo without annoying everyone else around me.
