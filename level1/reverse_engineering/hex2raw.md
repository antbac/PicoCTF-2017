The file we want to abuse is located in */problems/c69bcda4ca5a28fd9d18790fc763db73*.
Once we run the file we are asked to enter some bytes they give us.
The problem is that not all of these bytes are easily entered through a keyboard.
So what we would like to do is to enter these bytes in some other manner.

What I decided to go with was the *echo* command with the *-e* attribute.
This allows me to convert the bytes to *hex* and have the computer convert them to raw bytes for me.

All I have to do is copy the bytes they want me to enter and add **\x** in front of them.
Finally I pipe the output from the *echo* command to the program using the **|** sign.
This gives me the command:
```bash
echo -e '\x41\x6f\x1c\x79\x18\xf8\x3a\x4f\x19\x22\xd8\x6d\xf5\xe7\x83\x48' | ./hex2raw
```
