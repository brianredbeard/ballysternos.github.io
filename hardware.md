## Building the J5 Card
The card to plug into the J5 connector of the MPU primarily consists of a 74125 (quad line buffer), and an Arduino Nano. Several headers (0.1" F) are used and a switch to control whether the machine boots the original code or the new.  
  
The J5 connector on the MPU was designed as a diagnostic port. With access to all the data, address, and control signals, it's an ideal spot from which to take over control of the machine. The Arduino Nano has enough speed and memory for that task. The 74125 chip is used so that when the Arduino is not in use, some of the lines can be put into a tri-state mode so they won't affect the MPU's bus. This allows for the dual-boot feature.  
  
The board will look like this:
![Image](https://user-images.githubusercontent.com/36781010/95404330-bbb89780-08e2-11eb-9383-e1bc2b75af07.jpeg)
(the header to plug into J5 is on the back of this board)  
  
To construct this board, make the following connections:
![Image](https://user-images.githubusercontent.com/36781010/95404130-31703380-08e2-11eb-934e-25c1274028bc.png)
  
  
