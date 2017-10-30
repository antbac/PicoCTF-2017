We were given a short **pcap** file and asked to find the password that someone sent.

Opening the file in *wireshark* we can tell that the user has logged in using *HTTP*.
We can filter out the files not using *HTTP* by writing "http" in the filter bar.

Seeing as the user has logged in we can assume they used a *POST* request.
There is only one *POST* request sent, and checking it out we can find a username and password.

We can tell that the password has been *base-64* encoded thanks to the 2 equal signs at the end.
All we have to do now is to decode the password back to regular encoding.
