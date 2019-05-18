## Overview

       The smart glove is the primary part of the project as it is the part the user will be in contact with.  
  It consists a 433MHz transmitter, an accelerometer and a bluetooth transmitter all controlled by a  
  arduino nano.  This portion of the project accomplished 3 tasks: counting dumbbell curl repetitions,  
  relaying that count to the phone, and relaying it to the LCD.

	While building this there were a few issues that needed to be dealt with.  To get the accelerometer to count  
  reps an if loop was used to check if there was a significant increase in acceleration to detect if there’s movement  
  and to check if there were any other recent increases in acceleration to see if it is a seperate movement.  For the  
  433MHz the range was not quite what we hoped for and using an antenna or increasing power through a transistor did  
  not yield any noticeable improvement.  To solve that a better transmitter/receiver would be used in an  actual product.

	In order to connect to the phone, we first tried the JDY16 Bluetooth module. We have decided to move on to  
another Bluetooth module, the HM-10 when the JDY16 did not work. The advantage of HM-10 is that it could be connected to 
iOS devices which are more widely used in campus. Once this was connected the glove could send the rep count to the users phone,
they could then enter the weight they lifted with so the glove (arduino nano) could calculate the total volume lifted for the  
user to save to their phone. The rep count was also sent to a display for the user to see as they worked out, and here there was  
also a timer for the weightlifter to use.

	The overall problem this was trying to solve which was helping a person keep track of reps, time, and total volume lifted. 
  This transmitter did what it needed to in order to solve that problem. In the future this could be adapted to other exercises   
  to make this more viable as a product.