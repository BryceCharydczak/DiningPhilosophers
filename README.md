# **DiningPhilosophers**

This is a tool written in Python to visualize the Dining Philosophers problem; the timings are set to create eventual deadlock, but decreasing or removing the time of holding the second chopstick will greatly reduce the likelihood of deadlock.  This software could be used to help illustrate the dining philosophers dilemma to students and teachers alike in order to assist in learning/teaching a potentially confusing notion. 

# *Explaining the Process*

This implementation of the Dining Philosophers Deadlock scenario is developed using the graphics.py, threading.py, and time.py libraries. Graphics manipulation is limited to the mainThreadAction (graphics operations not supported outside of it) so the actions of the concurrent processes are not represented with 100% precision (as opposed to having all graphics manipulation done inside of the actual "eat" method). However, the program definitely is effective at representing the notion of the dining philosophers dilemma.


# *How To Use It* 

This is an explanation of how to use the program on Ubuntu 16.04. The project uses the Python3.5 interpreter and Ubuntu 16.04 ships with Python 3 and Python 2 pre-installed. To make sure your versions are updated, use 

sudo apt-get update
sudo apt-get -y upgrade


Now, you need to make sure you have the necessary python libraries. 

To get graphics.py, go to http://mcsp.wartburg.edu/zelle/python and download graphics.py

Open terminal, cd to /usr/lib

Change permissions of the python3.5 directory with: 

sudo chmod +x python3.5

Now, navigate to the directory you just downloaded the graphics.py library to. 

You'll want to move this libary to /usr/lib/python3.5 so that the python 3.5 interpreter can access it. 

Use the "sudo mv" command to do this. For me, the library was in Downloads, so from the Downloads/ directory I enter:

sudo mv graphics.py ../../../usr/lib/python3.5

Now, your Python3.5 interpreter has access to the graphics.py library.

The threading library should already be in Python's standard library so you don't need to manually install it. 

Open an IDE of your choice (we used PyCharm for development). 

Run the backendThreads.py class; 
when the graphics window appears, just click the window and watch the magic happen.

In order to adjust when the deadlock event happens, you can increase or decrease the very last time.sleep() statement in the dpsim.py file. 

Thanks for reading!



