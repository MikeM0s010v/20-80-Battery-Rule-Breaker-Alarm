-20-80-Battery-Charge-Percentage-Exceed-Signalizer-

Rough venv-python alarm for 20-80% battery rule. It simply reminds you to plug-unplug the power cable.  The programme starts as you login into your Linux user account..

Steps
1. Create venv folder. Put the python script and alarm wav-file in there.
2. Create a bash script that changes directory and runs the py-file.
3. Add modifications to your .bashrc-file.  

Enjoy! LOL


The program will work if you leave the terminal open while logining out or shoting down. There is also some time lag in python power_plugged attribute staus refreshing. Thus Xterm command and/or further sleeptime adjustments may be added or detalized.

CPU usage 
ps aux --sort=-%mem | grep -i '[p]ython'
user 2300  0.0  0.0 256060 17720 pts/0    S+   04:21   0:00 python alert.py

