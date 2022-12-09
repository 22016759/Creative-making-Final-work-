# Creative making: Physical Computing Project Blog!

# Introduction:

Overall, I think I encountered a lot of difficulties from coming up with the idea to completing the project. I felt a lot of pressure at first because I didn't have much contact with ARDUINO before, but fortunately I solved the problem step by step slowly and I felt happy that I actually made it. In fact, after the fourth week, I was in a deep state of fear and helplessness about the presentation I was going to do next week. I was happy to say yes for the sake of security, but this led to a lot of discussion until 4am trying to come up with a design that would work best, so as you can imagine we decided to go our own way in week 5! I probably came up with a lot of ideas, but to be honest when I put them into words I didn't feel confident, at first I was afraid that the design would be boring, and this struggle was a constant part of the process, but then I thought about my design over and over again and I felt that maybe it wouldn't be a meaningful design, but maybe it was a meaningful design practice for me.

I must mention that I had a lot of help from my classmates and teachers in this project. I started from not knowing anything, not knowing how to write code, not knowing how to laser cut, not knowing how to 3D print (although I didn't end up using 3D printing in my project), to finally knowing how to connect input sensors and control multiple output sensors, knowing how to use the laser cutting machine, knowing how to use the 3D printing machine, and how to use the 3D printing machine. Another small lesson I learned in practice is that it is best to solder expansion boards with the positive and negative terminals two rows apart (of course if you are very good at soldering you don't have to do this).

# Week 4

# Project Proposal:

# Concept:
Accepting and embracing the randomness and uncertainty of life.

# Project Name: BOMB BOX

# Keywords:

Unknown, Randomness, Indeterminacy, Unexpected, Surprise.

# Possible Inputs?

Ultrasonic sensor: Detects the approach of someone with an ultrasonic sensor.

Button: Or the whole device can be turned on with a button, consider a point signal, press and hold the button to inflate the pump and release to stop inflation.

pulse sensor: Detects the heart rate of a person when they engage the device, different people's physical reactions to unknown things.

# Possible Outputs?

LED: Visualisation of the heart rate and visualisation of the change in heart rate.

LCD: Reads the heartbeat value.

Buzzer: Provides an audible signal that the balloon is about to explode, creating a tense atmosphere.

Air pump: Requires a device to inflate the balloon.

The teacher's requirements were very simple, in terms of hardware, at least two input sensors and output actuators, and no restrictions on the subject matter. But I found it difficult and unrealistic to imagine, so I have been accumulating inspiration, sometimes from a quote, sometimes from a sudden feeling in my life, and then recording it as much as possible.

<img width="1203" alt="截屏2022-12-09 20 31 14" src="https://user-images.githubusercontent.com/119021236/206791153-48abd192-7297-4ec2-91c4-b20ad942e6d7.png">

The teacher's requirements were very simple, in terms of hardware, at least two input sensors and output actuators, and no restrictions on the subject matter. But I found it difficult and unrealistic to imagine, so I have been accumulating inspiration, sometimes from a quote, sometimes from a sudden feeling in my life, and then recording it as much as possible.

My inspiration is actually related to my recent life, when I first came to the UK, in just two months I experienced the unpredictability of the unknown because of some things, because of this I wanted to make a small device about randomness and unpredictability, we never know which one will come first, the unexpected or the surprise, just like in Forrest Gump, life is like a piece of chocolate, you never know what the next piece will taste like. At first I just wanted to put this unpredictability into a balloon that could not be predicted when it would explode, using ultrasonic sensors, the air pump would only inflate the balloon if someone was near, but when this balloon would explode and who would trigger it, we didn't know, including the person who was standing in front of the uitrasonic sensor, he didn't know how long it would take to inflate, he could only vaguely feel from the appearance if it was about to explode, I thought this whole process was interesting, the participants and the viewers were actually involved in this unpredictable experiment, then after thinking about it, I felt something was missing, I thought the mental activity of the process would be exciting too, so I made the participants' heart rate responses visual, so it seemed to complete it, perhaps the LCD display responds to heart rate, or perhaps I want to make a cap with a light on top of my head, where the heart rate is proportional to the flashing frequency of the light.

# Week5 

Design and planning

My task this week was to first identify what parts I needed, then buy them and find out how to use them. I then split the device into two parts, one to address the visualisation of the heartbeat and one to complete the balloon inflation.

This week I actually struggled with what features I wanted to achieve or how to go about matching the sensors and actuators, going back and forth with a lot of ideas, and because I had so many ideas I almost went off topic and ended up in a funk and forgot what I wanted to say most.

On the left below is my initial sketch, but after thinking about it I re-planned the design flow diagram and my teacher told me that I could simplify the device appropriately and not make it too cumbersome. So on the right I am posting the simplified schematic.

<img width="780" alt="截屏2022-12-09 20 39 31" src="https://user-images.githubusercontent.com/119021236/206792372-c01a3558-1ae6-498f-a749-c523b8b4c988.png">

Secondly, I am going to use the following two weeks to address the code for the heart rate sensor to trigger the LED and the code for the ultrasonic sensor to trigger the air pump respectively.

# Week6 

Experimentation

My main task this week was to write up and carry out some experiments on the heartbeat detection sensor.

At first I used the C19 heartbeat detection sensor and it detected my heartbeat very irregularly (must not be my problem), I thought there might be a problem with how I was using it, even though I looked up the introduction to using this type of sensor, I could still find that putting my finger on the small bulb and on a small protrusion on the left side both detected the rise and fall of the waveform, which made me even more unsure how to use it.

<img width="800" alt="截屏2022-12-09 20 45 32" src="https://user-images.githubusercontent.com/119021236/206793226-0d8fdc28-7484-4c63-a7aa-f9fd85ded2cd.png">

Later on monitoring my heartbeat was finally regular, and after researching the reason for this, the light emitting LED was above the finger and the phototransistor was below the finger, the phototransistor was used to obtain the emitted light flux, when the blood pressure pulsed through the finger there would be a small change in the resistance of the phototransistor, try to avoid stray light entering the phototransistor when detecting it.

<img width="802" alt="截屏2022-12-09 20 46 47" src="https://user-images.githubusercontent.com/119021236/206793397-0dcbc5f2-1d93-4b10-a47f-d424a315a924.png">


