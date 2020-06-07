The file with extension .c is the code that we use to program the Radio in the Raspberry Pi 3+\
Save the archives along with the songs in a USB Flash\
**It is important to remark that the sound files admitted in this program are .wav files which use one channel (mono) with a sampling rate of 22050 Hz**

Access to the Raspberry terminal\
Use PuTTY program to access the terminal by identify the ip address of Raspberry and later click on Open

Access the code stored in the USB Flash from the Raspberry terminal\
Log in with the Raspberry username and password\
Write two times cd .. and enter:\
then:\
cd media\
cd pi\
cd "Name of the USB Flash"\
To see the archives .wav and .c write ls and enter

To view the code write:\
nano radio_station.c

To compile the code write:\
gcc -lm -std=c99 -g -xc radio_station.c -o radio_station

To start the system of the radio station\
sudo ./radio_station "name of the wav archive".wav "frequency"\
Example:\
sudo ./radio_station b.wav 98.40
