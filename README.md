# Muad-Dib
RRCC Robotics Project


/*

The code at the lisan algaib main file/branch is the one we used and actually worked for the 2025 robot

stuff to improve would be IMU aoutocorrection, DONOT make the IMU actually storage info in the Arduino, it will either generate a memory leak (which will break the code) or will simply not work at all due to the small memory the Arduino has

the logic for this is that the initioal direction (in degrees or radiants) should be memoriesed when the robot turns on or reboots(resets), this value should NOT BE MODIFIED, put in the private section of the .h file and make it const just to make sure, this value will be the one the IMU will compare with once the object has been avoided, make sure that this new autocorrection code only activates once the object has been avoided (the sensors stop detection stuff),

also add a autocorrection to the code, so that the IMU can correct itself when going straight (if the robot is turning a lot when its supposed to go straight make it to stop and back up) and to make sure its going straight, this is the only situation a apart from the autocorrection of initial position, when the IMU should work, so in other words the IMU hsould only work dueing 2 situations when correcting its path to go towards the end of the circuit and when correcting it self when going in a straight line




*/
