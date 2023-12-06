#Idea
I'm trying to generate a control that interacts with music and lights through sensor control, and I'm not sure if this idea is feasible. 

I want to combine our previous music visualization ideas, in the p5js part of the creation of a visual image of the music, and then to present the music waveform changes, or call some other library form to combine the music visualization, and then at the same time I don't know if it can be achieved, I want to let the Arduino to control the light flashing according to the music waveform. 

The general idea is to analyze the waveform, then the led blinks at the same time, or light up according to the order, or have time control, time delayed lighting. The user can switch between different light modes via potentiometers or buttons. 

chatgpt's idea is that the user can manipulate the music by changing the state of the sensors (e.g. blocking light or applying pressure).


[![GgIGQR.jpg](https://imgpile.com/images/GgIGQR.jpg)](https://imgpile.com/i/GgIGQR)

more IDEAS - 
1. 
Here I'm thinking about giving users the ability to directly intervene in the interactive effects of lights and music. I came up with this idea based on the photosensors I saw in class
For example, they could pause or change the tempo of the music by blocking the sensor with their hand
[![GgIx7g.jpg](https://imgpile.com/images/GgIx7g.jpg)](https://imgpile.com/i/GgIx7g)

2.
Based on what I've seen in class, I'm still thinking about what would happen if I used the p5js library to draw graphs based on the music by first using a computer, and then when the user covered the photoresistor or potentiometer with their hand, the waveform made a change or changed the pattern a little bit, and I don't know if that's feasible.
[![GgIDlr.jpg](https://imgpile.com/images/GgIDlr.jpg)](https://imgpile.com/i/GgIDlr)



#More
This code is my very first experience and I've encountered very many difficulties and problems
The code of my basic framework is this assignment submission, but relatively I want to change it to interact through the effect of lights.
I would like to have a photoresistor to control four led's, first I should need the p5.sound library to analyze the file waveforms
Need ArduinoJson for serial communication. p5.js for visualization.

The point is that the size of the circle is changed interactively by using the arduino to read the value. Here are the possibilities for interaction

My interaction is that first the page draws circles of the same size with music, then by changing the value of the photoresistor (the flash passes through), the circles that appear in the interface change to different sizes.
Then by changing the value of the photosensitive resistor (through the flash), the circles that appear on the interface become different sizes, and then at the same time the brightness of the led light decreases. Regarding the user experience, I think it could be done either by covering the photoresistor with your hand, or by using the flash.
covering the photoresistor, or by using a flash. If that fails, my backup plan may be to simplify the process or remove the light part.

The general idea is
Target users could be those interested in interactive art or educational tools.
Interaction involves altering light exposure to the photoresistor (using hands, flashlight, etc.) and observing changes on-screen and LED brightness .

This time I found a lot of difficulties in reading my libraries, I did it through wifi but I was reminded of the problem with my firewall settings that the ip is not uniform, but the serial libraries were never read.
But the serial library was never found. I changed it several times and it keeps reminding me
! [GgomYW.png](https://imgpile.com/images/GgomYW.png)
Then the port issues came up, and these are things I need to learn or else it totally affects my assignments

Here's my thought process.
! [GgAidi.jpg](https://imgpile.com/images/GgAidi.jpg)
It should run along the lines of
! [GgAcgk.jpg](https://imgpile.com/images/GgAcgk.jpg)
I made a simple one, and my desired rendering is this!
[GgkuNk.png](https://imgpile.com/images/GgkuNk.png)

I think this kind of human-computer interaction reminds me of the data visualization mentioned at one point, where I converted the photosensitivity to a visualization of the changes, with the circle size representing the value passed. I realize that light changes are hard for the human eye to see, but it makes more sense if I make it more intuitive to see the problem through simple geometric changes in size. Although it is only a change in light, I think this basic idea can be extended to more places. For example, for people who are not highly photosensitive, or for testing in some places. The significance for me is that I've been hoping to do some visualization, and I was hoping to add some music detection visualization per se, and this time I added light visualization (which is hard) but I hope it works.











