<h1>Streamlining SSH Configuration</h1>

![Image](SS1.PNG)
<br> I opened the **.ssh/config** file through the VS terminal, then I edited the config file through VSCode.

![Image](SS2.PNG)
<br> I created an ssh shortcut by adding myself to the host ***ieng6.ucsd.edu***. This allows me to login to the ieng6 machine faster by typing ```ssh ieng6```; a password is no longer necessary to login.

![Image](SS3.PNG)
<br> With that same shortcut that I created earlier, I am able to use it when transferring files over to the ieng6 machines. 
<br> The input follows as ```scp [FILE] ieng6```



<h1>Setup Github Access From ieng6</h1>

![Image](SS4.PNG)
<br> I created a **public SSH key** for my PC and I stored it in my Github account.

![Image](SS5.PNG)
<br> The private key that was made can be seen when I log into the ieng6 machine and ```cd .ssh``` then ```ls``` to show the one of many keys.

![Image](SS6.PNG)
<br> On the ieng6 machine, I removed a file in markdown-parser using ```git rm test.txt```, then I committed the change using ```git commit -m "removal"```.



<h1>Copy Whole Directories With scp -r</h1>

![Image](SS7.PNG)
<br>Show copying your whole markdown-parse directory to your ieng6 account.

![Image](SS8.PNG)
<br>Show logging into your ieng6 account after doing this and compiling and running the tests for your repository.

![Image](SS9.PNG)
Show (like in the last step of the first lab) combining scp, ;, and ssh to copy the whole directory and run the tests in one line.<br>