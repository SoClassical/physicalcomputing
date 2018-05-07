# Final Project

## Coinless Jukebox

#### The finished product: https://youtu.be/VYbEmWk-_nk

#### To make this, I used 1 momentary switch, four LEDs, four paper cylinders to cover the LEDs, an Adafruit audio fx sound board, two breadboards, and an Arduino Uno. Originally, I wanted to use four different colored LEDs, but they were not as bright as I wanted them to be. I ended up using three blue and one white LED because I did not have a fourth blue one. I also used a Cricut to cut out four pentagonal cylinders to cover the LEDs.

#### The concept of this project is that when the box is closed, the momentary switch is pressed. When the box is opened, the change from the switch being pressed to being not pressed triggers the sound board to play a song. When the song is played, a LED will illuminate indicating which song is playing. Each time the box opens, a random song will be selected, so there is a possibility that the same song will be played.

#### The songs in the jukebox are:
#### 1) Jaws theme song
#### 2) Harry Potter theme song
#### 3) Star Wars theme song
#### 4) Simpson's theme song

### The process:

#### I first planned out what I wanted to do on a sheet of paper. I originally wanted to use a piezo, but my professor suggested that a sound board would elevate the project, and it did. Instead of 8-bit sounding music that couldn't produce rhythm, I was able to play higher quality songs without inputting all the notes myself. Because I had no idea what to do with the sound board, I first assembled the breadboard for the switch and LEDs. I quickly realized that my breadboard was not enough, so I had a separate breadboard for the switch and sound board. Using what I had so far, I wrote the code for turning on the LEDs when the switch was not pressed, but was unable to move on from there until I had figured out how to use the sound board. In the meantime, I had found a box that could act as my "jukebox."

#### Learning how to use the sound board was more difficult that I imagined. For starters, I could not find anywhere that taught me how to use the sound board besides the Adafruit website. I was able to save music onto the sound board by saving the files as .WAV files. However to get music to play was beyond me. The tutorial said that if the sound board received power and the music files were named correctly, music would start playing automatically, so I tried to use my portable battery pack. I also read in the tutorial that some battery packs would automatically turn off after some time if not enough current draw was detected, so I hoped mine would be okay. Unfortunately, my portable battery pack turned off within 30 seconds and no music played. Afterwards, I tried two more battery packs that I had in the house, but they too turned off without playing music. In my desperation, I asked a friend to borrow her battery pack> To my relief, it worked! I was finally able to power the battery pack. However, still no music played.


#### The switch would not play any song no matter what I did. To fix this problem, it was suggested to me to use a trigger for the sound board. The trigger used and modified was found off of GitHub (https://gist.github.com/stonehippo/308a5f5c49d4981ac976#file-simpleaudiofxtrigger-ino-L33). With this change, when I turn on the battery pack, the first song would play. Still, I could not get the other songs to play.

#### I wanted the songs to play randomly, but also be activated by the switch. By assigning each song to a different number in the code, when the random (not truly random) number was generated, in theory, the corresponding song would play. Through this method, I was able to randomize the order of the songs.

#### I realized that the other songs would not play because I had named the .wav files under the wrong name. Although I do want the songs to play randomly, I still wanted it to be controlled through the switch. Therefore, I had to rename the files. After renaming them to the basic trigger name, I was finally able to hear the other songs when their number was generated.

#### Last piece of the puzzle was finding a way to press down on the switch while the box was closed. I originally wanted to affix a dowel the top of the box that would press down on the switch when the lid closed, but because the switch was so small, there was a huge chance the dowel would miss the switch. Instead, I placed a bamboo stake for orchids on the switch and secured it with some string and tape. Because the stake was a little longer than the height of the box, whenever the lid was closed, it would press down on the switch.

#### Using the box I had found, I covered up the breadboards, wires, and Arduino with a sheet of thicker paper. In the paper, four pentagonal holes were cut to fix the LED covers. On the LED covers, I drew icons that represented the song, then cut up slits so that light could escape through when the LEDs illuminated. With that, my Coinless Jukebox was complete.

#### If I had more time with this project, I would want to change a few things. First off, I would make a more stable way to press down the switch because it was a little wobbly. It worried me that the music would not activate after opening the box because of it. I would also want to change the code so that a song would not play twice in a row. During the interactive media show, it seemed like people were a little disappointed when the same song played twice, even though the songs played randomly. I would also want to change the Harry Potter theme song to a louder song. Even with speakers, the song was too quiet and could not be heard during the show.
