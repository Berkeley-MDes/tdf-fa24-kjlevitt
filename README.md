## Week 14 11/28/2024-12/5/2024
With the fabrication of the tiles completed, we moved on to trying to figure out how we would like all of the tiles to be displayed together. We knew that we would like them to be positioned in a grid pattern but were not sure exactly how to do this with the positioning of the tiles on the servos themselves. It took me a while to come up with a good design for this. Eventually I came up with the idea of creating shelves that would have cutouts the exact size of the servos in order to keep them in place when they are rotating. These shelves would have to be positioned far enough away from the front so that the arms connecting the servo to the tile would sit flush with the front of the box, hold the servo at the correct height so that the tile is in the correct place in the grid, and allow for enough clerance on all sides for it to rotate properly. When I had an overall design completed for this, I then was tasked with figuring out how all of these pieces would be able to fit together properly so that we could laser cut all of the boxes in the most efficient manner. Most of our connections ended up being through adding mortise and tennon-esque joints. 

<img width="400"  src="assets/Fusion grid front.jpeg"> <img width="400"  src="assets/Fusion grid back.jpeg">

Fusion model of the enclosure

<img width="600"  src="assets/Cardboard grid.jpeg"> 

We laser cut a carboard model of the design first to test that it would all fit together how we wanted

<img width="600"  src="assets/Wooden Grid.jpeg">

After verifying that all the pieces would work together, we moved to laser cutting all four of the enclosures out of wood

## Week 13 11/21/2024-11/28/2024
This week we started out by figuring out how to get the right power in order to have all sixteen of our servos rotating properly. We determined that it is necessary for us to have 5 volts running to our system but needed to supply approximatly 0.5 amps per servo that we wanted to use. Thus we decided that the best way to accpmplish this is to have a power supply running from a wall outlet that gives us 5 volts and 10 amps to our system. With the correct power we began testing out the servos to make sure that we could have them all functioning at the same time. We quickly found that even with the increased amperage all of the servos could not rotate simultaneously but when we had them operating in a wave motion they worked properly.

https://github.com/user-attachments/assets/db21dcaf-c05e-4057-b344-9306516fe7c7

With the servos operational we moved onto adding in the proximity sensor. This will be used so that the servos will be stationary when the person is far away and as they approach our installation the servos will begin to move in different patterns. Our original idea was to use three different proximity sensors so that it would be able to see which part of the display they were standing in front of. In order to use more than one of the proximity sensors, we needed to switch to using the PIR motion detector instead. Since this sensor can see for a much longer distance than the other sensors, I also worked on implementing a potentiometer with the servo so that we could adjust the sensitivity and distance that the sensor can read.

https://github.com/user-attachments/assets/354a1e0f-f01f-472f-ae5d-aaf99f428427


In addition to working with the motion sensor and servos, I was also helping to assist Roopa with the creation of the rotation of the tiles. We were having a hard time figuring out how to get them to have the motion that we wanted in a easy to print way. I had thought of an idea of being able to utilize screws as the axle points for the rotation of the arms with the servo and the tile and Roopa was then able to implement this into her design and fabricate all of the tiles.

https://github.com/user-attachments/assets/21388f41-ff66-452e-8502-b2bc145d1e9b

## Week 12 11/14/2024-11/21/2024
## Week 12: Report 1
This week I worked on creating a proposal for the final project. Since I had previously identified that I would be working in a group with Sylvie and Roopa, we had a broad idea of the compoents we had to work with and what we would like to do with them. We had previously discussed using a matrix of servos in order to create an interactive art piece that would utilize sensors in order for the user to manipulate its outputs. From this we all created our own idea of how this would function in our proposals. During the pin-up session, we discussed each of our ideas and decided on using mirrors to be rotated by the servos.

Pin-up proposal

<img width="600"  src="assets/Project4PinUp.png">

For our interaction piece we will utilize proximity and heart rate sensors in order which will create movement patterns based on the inputs by the user. The idea for our project is inspired by the work of Daniel Rozin, whos work we all found particularly interesting and has many pieces utilizing various different mirror material being manipulated by electronics.

Example work of Daniel Rozin

<img width="600"  src="assets/Project4Inspo.png">

As we have started thinking about how to execute this, I anticipate that the main problem we may run into it in providing enough amperage to power all 16 of our servos. In beginning to do some baseline calculations and research we have found that we anticipate needing at least 10 amps in order to power all of the servos appropriatly. Our initial idea is to utilize a variable power supply in order to provide this. 

## Week 11 11/07/2024-11/14/2024
## Week 11: Report 1
This week I was focused on writing out my project 3 report. In this, I go deeper into the results that were gathered of the different demo experiments along with my final experiment. In working through this I was able to gain a better understanding of how LLMs in general function and how to improve upon the responses that were generated by my agents through addition knowledge sets and adjusting the parameters. In this, I ran each of my experiments through a variety of questions in order to better analyze how they were working. In the end, I was able to document the process that I went through along with illustrating the architecture and system process behind my final chatbot. If I were to continue this project into the future, I would like to work to figure out why some of the shortcomings on answering questions like names of participants and advisor were returning incorrectly and see if adjusting the knowledge sets and/or parameters would allow for it to be able to answer questions that are located in the charts and graphs of my report.

Process Diagram

<img width="600"  src="assets/LLMProcessDiagram.drawio.png"> 

System Architecture

<img width="800"  src="assets/LLMSystemArchitecture.drawio.png">


## Week 10 10/31/2024-11/07/2024
## Week 10: Report 1
This week I worked on extending the initial four tutorials into my own idea. My project was to create an LLM that could answer any questions about my senior design project, the Anti-Drowsy Driving Assistance system (ADDA). Since the initial name of our team was "Project Kiwi" which stuck with us throughout the rest of the project, I decide to make my LLM respond as a Kiwi bird named Adda who talks to you in a New Zealand accent. In order to do this, I needed to give the LLM information on my project. I decided to give it three sets of knowledge: our 78 page final deliverable report, the contents of a webpage that we had created in order to showcase our product, and all of the minutes that we had taken over the course of this ten month project (this was 64 days worth of minutes). With these three knoweldge sets I felt that it gave a comprehensive understanding to the system of both how our final product operated and the process we went through in order to get there. 

<img width="400"  src="assets/kiwi car.png"> <img width="400"  src="assets/Kiwi_LLM.png">

Once I had setup the framework for my model and input in all of my data, I played around with adjusting the temperature and chuncks for each knowledge set until I was getting answers that I was satisfied with. I asked it questions like "What does the system do?" and "How does the alert method work?" and it was able to give me pretty good answers back.

<img width="400"  src="assets/Kiwi_system_question.png"> <img width="400"  src="assets/Kiwi_alert_method.png">

In working with it though, I did find some pitfalls in the LLM that I could not figure out how to fix. The first one being that it could not answer to who was involved in this project eventhough all nine of our names are explicitly listed multiple times throughout the three knowledge sets that I provided to it.

<img width="400"  src="assets/Kiwi_name_prompt.png"> <img width="400"  src="assets/Kiwi_deliverable_front.png">

I also found that it was not able to give proper answers or sometimes answers at all about information located in tables or charts. While it is able to parse plain text well this is a pitfall for analyzing things like my deliverable report for information.

## Week 9 10/24/2024-10/31/2024
## Week 9: Report 1
The first part of this week I was focused on writing the report for the second project. 

Once this was complete, we moved into starting on project 3. In doing so, I started working through the tutorials for creating my agent. i do not have any pervious experience in building a LLM so this was a very new task for me. It took me a while to get through the tutorials as I kept running into diffefrent errors that would occur as I was trying to get my agent to work correctly. Eventually, I was able to get through all of them and have my agent working as intended.

For the last tutorial, I ended up adding in both the content from my github and my resume in order for it to be more in-depth of its knowledge about me.

<img width="800"  src="assets/GPT_Experiment01.png">

## Week 8 10/17/2024-10/24/2024
## Week 8: Report 1
This week I was focused on completing Project 2. At the beginning of this week, we had realized that we needed to integrate one more input sensor into our penguin. The idea that we came up with was in using the accelerometer in order to turn on an led when it is shook. This way we could implement the accelerometer into the hand of the penguin and when the user shakes his had, an LED will turn on. This was fairly straightforward and I was able to implement this using the accelerometer sensor and a singular LED. 

https://github.com/user-attachments/assets/4688d5e4-5cd8-4a99-82f6-91de8d1308bf

Once we had this complete, I compiled all of the separate code into one system. This way our penguin would function by having the ultrasonic sensor to turn on the servo when a person is within the correct range and have the accelerometer to turn on the LED running on the same photon. 

After I had this code running sucessfully for both of these sensors, we really wanted to utilize multiple LEDS to display a heart on the penguin instead of having just one. I first started out with trying to get the NeoPixel Featherwing that I had from another project to function with the photon. As there is no library supported for this on the photon it turned out to be quite difficult. I tried altering one of the libraries that is offered but this only caused the photon to turn on and spasm with random lighting no matter what code I gave to it. 

<img width="400"  src="assets/NeoPixel.jpeg">

As I could not get this to work, Kaylee had an LED dot matrix that she gave to me to try instead. I found a library for the photon that looked promising to make this work but no matter what I tried I could not get it to compile with the code that I had. Even using the example code that was offered within the library and going through the library myself to see the functions I could not figure out why this was not working. 

With two different LED matrices not working I decided to give it one more try, using the DotStar Featherwing. I assembed this together as per the instructions that I was given and the dowloaded the example code that Jeff gave to me in order to run on it. Even with this I still could not even get it to turn on at all. So with this, I needed to give up on the LED matrix and we instead transitioned to having a OLED screen in the center of the penguin to show the message and heart and then having a regular LED to light up on the top of his head. 

With putting the penguin together we ran into many more issues mostly around unreliability of the photons functioning. This was very frustrating but I am still proud of the product that we were able to come up with in the end. I would really like to try and get this project to a fully reliably functioning state in the future along with getting one of the three LED matrix boards that I now have to work with the photon.

<img width="400"  src="assets/Pebble.jpeg">

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/3kVe9mILyTI/0.jpg)](https://youtu.be/3kVe9mILyTI)

https://youtu.be/3kVe9mILyTI

# Week 7 10/10/2024-10/17/2024
## Week 7: Report 1
This week was lots of focus on working on project 2. We first worked together in order to come up with a idea for the project that we wanted to work on that fulfilled the requirements. Our idea consisted of two main components. a button that can be pressed remotly in order to trigger an led light to turn on and a model of a beak which would open when a person is close enough to the proximity sensor. 

Once we had our initial idea of what we wanted to do, I started with first working on creating a model for the beak. During class, we had created an initial cardboard model of what we thought a possible design would be. From this, I worked on creating a 3d model of this that would have screws in order to act as the hinges for the mouth to open and close. 

<img width="400"  src="assets/Beak1.jpeg"> <img width="400"  src="assets/Beak2.jpeg">

## Week 7: Report 2
Once we had an initial base for what we wanted the beak to look like, I moved into working on trying to make the proximity sensor and servo motor function together. I first made the RGB led function with the proximity sensor in order to more easily test out that my code was functioning correctly. I had it so that when proximity was between 80 and 20 the led would turn green, when proximity is closer than 20 it will turn red, or else it would turn blue. 

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/AW2mKCWXW2g/0.jpg)](https://youtube.com/shorts/AW2mKCWXW2g?feature=share)

https://youtube.com/shorts/AW2mKCWXW2g?feature=share

Once I had this code working I tried to adjust it for the servo instead. I thought that this would be simple, as I would just have to change the led to making the servo write to a specific angle. When I did this, nothing occured. I tested to make sure that both the proximity sensor and the servo were functioning independently but do not work together. I tried troubleshooting the code in multiple different ways including having the proximity sensor using the particle to power it and the servo being powered off of the external battery and making the baud rate slower. Neither of these worked so I tried using the ultrasonic sensor instead. I used the same framework code but replaced the proximity sensor with the ultrasonic one and it worked on the first try. 

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/tiwMlrAHarw/0.jpg)](https://youtube.com/shorts/tiwMlrAHarw?feature=share)

https://youtube.com/shorts/tiwMlrAHarw?feature=share

The last thing that I worked on for this week was in improving the design of the beak. I made the hinges on which the screws move the top and bottom of the beak integrate into the design better. On the bottom portion of the beak I added in a bunch of small holes that will allow for it to be sewn into the stuffed penguine. For the top beak, I added in a part that sticks out with a hole in it so that it can be attached to the servo in order to open. 

<img width="300"  src="assets/Beak_Assembly.jpeg"> <img width="300"  src="assets/Beak_bottom.jpeg"> <img width="300"  src="assets/Beak_top.jpeg">

# Week 6 10/03/2024-10/10/2024
## Week 6: Report 2
This week has consisted of very much frustration for me reguarding the photon. On Saturday afternoon I was working on testing out the different sensors with the photon in Jacobs. Once I had finished I decided to go home and continue ,y work. When I plugged in my photon at home it began to continually blink blue, not able to access the wifi. Since this time I have spent many hours going in circles trying to troubleshoot and get my photon to connect to the wifi. This blinking light has become a source of frustration for me and I have not been able to connect or flash anythng to the photon since Saturday. I have tried resetting, restoreing, and running many different commmands in the CLI but nothing seems to work :(

https://github.com/user-attachments/assets/9f45accc-5c95-4933-b94d-4a51349b09c0

## Week 6: Report 1
In completing the homework for this weekend I needed to solder the SparkFun shield. This turned out to be a bit more complicated due to the fact that I initially soldered the connectors to the board upside down. 

<img width="500"  src="assets/soldering1.jpeg">

I only realized this once I had finished soldering all of the pins and tried to attach it to the photon and it did not fit. I have never desoldered before but it was now necessary for me to figure out how to. Thankfully Gary was able to asist me in what would be the best way to remove the connectors. Unfortunatly, this involved needing to basically break it apart in order to fix it. The first thing that I needed to do was carefully pry the plastic cover off of the pins. Once this was off I used the soldering iron to heat up the solder that I had placed on each of the pins and once it was liquid I used tweezers to pull the pins out of each of the holes. With the pins removed most of the holes were still filled with solder. I then used the soldering iron again to heat up the remaining solder and used the solder sucker to get it out. 

<img width="500"  src="assets/soldering2.jpeg">

After the solder was removed from all of the holes, Gary gave me new pins to resolder to the board the correct way. 

<img width="500"  src="assets/soldering3.jpeg">

Now, with my board assembled correctly, I worked on attaching the sensors. The first one that I did was the MPU-6050. For this, I had the gyroscope enabled. This allowed for the position values to be printed in the serial monitor. It can be seen that as I rotate the device the numbers of the position change accordingly in the x, y, and z directions.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/fSxvDcgkZ8c/0.jpg)](https://youtube.com/shorts/fSxvDcgkZ8c?feature=share)

https://youtube.com/shorts/fSxvDcgkZ8c?feature=share

After this, I used the APDS 9960 board with the proximity sensor enabled. Here it is set up to detect the disance that an object is away from the sensor. As my hand moved closer to the board it can be seen that the proximity value increases. 

https://github.com/user-attachments/assets/d0a4d691-6716-4919-ad94-ed5e3ce76004

# Week 5 09/26/2024-10/03/2024
## Week 5: Report 2
This week I worked on going through multiple of the tutorials in order to familiarize myself with many of the components that were given to us. The first tutorial that I worked through was in getting a led to flash at a varying frequency that increases when a button is pressed. The led starts off flashing very slowly and every time the button is pressed, this gets faster until it meets a threshold in which it then loops back to flashing at its slow rate.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/kGs-4r-hwNw/0.jpg)](https://youtube.com/shorts/kGs-4r-hwNw?feature=share)

https://youtube.com/shorts/kGs-4r-hwNw?feature=share

The next tutorial was in using a pressure sensor and RGB led. The sensor uses the pressure that is applied to it to create an electrical signal. This signal is then used by the led to determine the colors that it will produce. Varying the pressure then changes the colors with the led turning white when the highest pressure it can sense it provided. 

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/E6OdYqmTeAg/0.jpg)](https://youtube.com/shorts/E6OdYqmTeAg?feature=share)

https://youtube.com/shorts/E6OdYqmTeAg?feature=share

The last tutorial that I did was in using the potentiometer to adjust the angle that the servo motor rotates. I decided to use the potentiometer in this tutorial instead of the accelerometer and edited the provided code for this. The potentiometer allows for the rotations provided in it to correspond to the angle that the servo rotates between 0 and 180 degrees.

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/bO__WhVxM3w/0.jpg)](https://youtube.com/shorts/bO__WhVxM3w?feature=share)

https://youtube.com/shorts/bO__WhVxM3w?feature=share

I enjoyed working with the electronics and refreshing myself on how many of these components function together. I had wanted to have the oled board function but could not figure out how to get the proper libraries in order to making it function. I intend to continue working on this so that I can figure out how to use this. 

## Week 5: Report 1

Over the weekend I worked on better understanding the Photon. The first step that I went through was getting it connected to my home wifi which I found to be quite simple to do. 

Once I had it connected I proceeded through the provided into codes. The first two provided codes were to print Hello World in the serial monitor, first as one line and then printing each individual letter. 

<img width="600"  src="assets/HelloWorld_print.jpeg">

https://github.com/user-attachments/assets/ec2d6ab2-feb0-4c5e-88bc-0137bc9e7265

After completing this I worked on wiring the breadboad to include a button. This button when pressed would cause "button pressed" to be printed in the serial monitor and vary the speed at which "Hello World" was being printed in the monitor. Each button press corresponded to the system choosing a random speed at which this would be printed. 

<img width="600"  src="assets/breadboard_pic.jpeg">

https://github.com/user-attachments/assets/eb2836c5-e020-4b1c-9784-9a9fb397e160

To keep adding onto this, the next two codes allowed for first one and then two leds to be connected. These would then flash at the same randomized rate that the letters were being printed at. 

https://github.com/user-attachments/assets/1e26b466-a87f-4608-9a75-edebbcd6c47a

After I had gotten through all of these provided codes I decided to play around and edit them. I took out the randomization in the speed with each button press. I then changed it so that everything was waiting for the button to be pressed to commence. Once the button is pressed both "botton pressed" and "Hello World" will print once in the serial monitor. After this occurs the green led will flash and then the red led. The system then waits for the button to be pressed again before running through the functions. 

https://github.com/user-attachments/assets/b42dc26d-ff08-4e06-9d0c-018f9203a566

# Week 4 09/19/2024-09/26/2024
## Week 4: Report 1

My main focus at the beginning of the week was in finishing the report for project 1. I am overall satisfied with the product that I was able to make for this project and have even actaully started using it to call my friends. I was surprised by how well recieved my phone stand was by my peers and might go back and edit this design to improve it given their provided feedback.

As we move into our next project we were tasked with creating an ecosystem map. In mine I chose to map out some of the most common ways that I interact with devices in a typical day. My diagram is separated into three main categories: my watch, cell phone, and laptop. Once I listed out all of the main ways that I use these devices I grouped them into four distinct categories of tasks: fitness, productivity, entertainment, and communication. As can be seen in my diagram, there is quite a lot of overlap between what I tend to do on my phone and computer, with most of these living in the categories of entertainment and communication. 

When looking at my watch and phone there is not nearly as much overlap. The ones that do exist are all in the category of fitness (with my alarm and time being an outlier). I would not necessarily consider my watch to be a "smart watch" as it is designed primarily for activity tracking. It has functions such as being able to tell you the weather and if I get a notification on my phone but I have these features disabled as they don't seem very effective as you need to continually synch your phone with the watch in order to have them function. Thus, outside of regular telling the time I utilize it pretty much only for tracking my runs and activity. This also expalins why there are no real overlaps between my laptop and watch that I could think of that I do on a regular basis.

<img width="600"  src="assets/Ecosystem Mapping.drawio.png">

# Week 3 09/12/2024-09/19/2024
## Week 3: Report 1

This week I focused on creating my phone stand using Grasshopper. The idea behind my design was that when I use my phone for video calls with my friends I tend to run into the issue of my phone battery dying. When this happens it means that I must hold up my phone for the duration of the rest of the call. This tends to get quite annoying so I created this stand so that it can hold up my phone while also being able to be plugged into the charger. 

<img width="300"  src="assets/PhoneStandGrasshopper.png"> <img width="300"  src="assets/PhoneStandRhino.png"> <img width="200"  src="assets/PhoneStand.jpg">

My design was challenging to create as it contained three different parts fitting into one another, unfolding at the appropriate angles and containg properly sizeed clearance holes for fasteners. In addition to just the composition of my design I also wanted it to be compact, foldable, and as thin as i could make it. 

<img width="300"  src="assets/Phone Stand Final.jpg"> <img width="300"  src="assets/PhoneStandInUse.jpg"> <img width="300"  src="assets/Phone Stand Pieces.jpg">

overall I am pleased with the design that I created but if I were to go back and edit it I would make it slightly less wide in order to support the phone better and adjust the angles of the arms slightly.

Here is the link to the video that I made going more in-depth into the design of my phone stand: https://youtu.be/kYWouX_ynT8

# Week 2 09/05/2024-09/12/2024
## Week 2: Report 1 #

I started off with making a chart of what I thought to be the different portions of the example Grasshopper file and how this was made into the different parts of the model.

<img width="500"  src="assets/Grasshopper_chart.png">

From looking at the provided model I was still confused on how many of the different operations in Grasshopper would function as I have never used this software before. I ended up finding a tutorial online of someone walking through step by step on how to create a parametric box using Grasshopper. I found working through this tutorial to be very helpful in starting to get down some of the basic commands.

<img width="500"  src="assets/ParmBox_Rhino.png"> <img width="500"  src="assets/ParmBox_grasshopper.png">

With my baseline understanding of Grasshopper I decided that I wanted to try and make something of my own in order to see if I could apply what I had learned properly. I chose that the gearbox that I had previously made (and modeled in Fusion360 before) would be a good thing for me to try and get the overall shape down of. It took some trial and error and working through some things but I was able to get the overall shape correct. Trying to get the hole cut-outs in the bottom plate is a work in progress which I have not yet figured out how to do. 

<img width="300"  src="assets/IMG_4759.jpg"> <img width="600"  src="assets/GearBox_Rhino.png">

<img width="500"  src="assets/GearBox_Grasshopper1.png"> <img width="500"  src="assets/GearBox_Grasshopper2.png"> <img width="500"  src="assets/GearBox_Grasshopper3.png">

---

## Week 2: Report 2 #

I decided to continue editing the model of the gearbox that I had started eariler in the week. In order to complete the overall body of it I needed to add holes in both the bottom plate and the face of the rectangular portion. I played around with the solid difference tool but I cannot get the holes to go all the way through the part.

<img width="600"  src="assets/GearBox_Rhino2.png">

---

# Week 1 08/29/2024-09/05/2024
## Week 1: Report 1 #

For this week I had a bit of a difficult time in deciding what I wanted to make. Whle trying to come up with something that I could design that would be useful for me I observed many of my classmates making Cal themed objects for their design. I decided that I wanted to try and make a functional yet fun object while being tangentially related to Cal. Thus, I decided to design a cartoon bear holding a bowl. 

The first step in my process was to create a rough sketch of what I wanted it to look like. I wanted the bear to be sitting down and holding the bowl between his arms. An image of my initial sketch can be seen below. 

<img width="200"  src="assets/IMG_4742.jpg">



With an initial rough layout of what I wanted my design to look like I next moved into creating a 3d model of my design. Since I knew that the design of the bear would be a bit more freeforme I thought that belnder would be the most ideal way for me to be able to model it. The bear and bowl are made up of majority spheres that have been resized and manipulated in order to create the figure. The model that I created for the bear ended up looking more like a teddy bear than a cartoon one that I had originally envisoned in my head. 

<img width="400"  src="assets/Screenshot 2024-09-04 015755.png">



Once I had gotten my model to a point where I was happy with it I exported it from Blender and put it into PrusaSlicer. Here I scaled up my model and added in the supports. I was a bit suprised a how small I needed to make my model in order for it to print in a reasonble amount of time, being that a small model would take about 5 hours.

<img width="400"  src="assets/Screenshot 2024-09-04 015837.png">



After this, I proceeded to print out my model, wait for it to finish, and then remove all of the supports and clean it up. When the small version of my design had finished I ended up scaling it up to print larger so that I would actually be able to have it hold things. Pictures of this process and my finished product can be seen below.
 
<img width="300"  src="assets/IMG_4738.jpg"> <img width="300"  src="assets/IMG_4739.jpg"> <img width="300"  src="assets/IMG_4741.jpg"> <img width="300"  src="assets/IMG_4744.jpg">



With the time that I spent on this model I am content with how it turned out. I think there are multiple ways in which I could improve this and make it overall better. For the design of it I wish I had made it look a bit more like a real bear than a teddy bear plus my original plan also included having the Cal logo imprinted in the back of the bear.

## Quick Links, compiled here for your convenience: ##

- [TDF Wiki](https://github.com/Berkeley-MDes/24f-desinv-202/wiki) - the ultimate source for truth and information about the course and assignments
- [Google Drive Folder](https://drive.google.com/drive/u/0/folders/1DJ1b6sSDwHXX6NRcQYt10ivyQSgU0ND6) - slides and other resources
- [bCourses](https://bcourses.berkeley.edu/courses/1537533) - where the grading happens
- [Weekly Submission](https://docs.google.com/forms/d/e/1FAIpQLSewDzOzJZBlv70a4e1WoBsbwWCmCf5Hita4sCap24KXJ6EgyA/viewform)
