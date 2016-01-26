# LEDchika
The program is to blink an LED with a Raspberry Pi
Source code below--------------------------------


＃include<wiringPi.h>

＃define LED_PORT 4

int main (){
	
	int i;

	if(wiringPiSetupGpio() == -1)return 1;
	pinMode(LED_PORT,OUTPUT);

	for(i=0;i<10;i++){
	//led on
	digitalWrite(LED_PORT,1);
	delay(500);

	//led off
	digitalWrite(LED_PORT,0);
	delay(500);
	}
	return 0;
}
-------------------------------------------------


↓↓VIDEO URL

https://www.youtube.com/watch?v=1QTac9_S1B4&feature=youtu.be
