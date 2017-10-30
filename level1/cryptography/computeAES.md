We are given an encrypted text and the key as well as the mode and algorithm used to encrypt the text.
We're also told that the text and key is encoded using *base-64*.

The easiest way to solve this problem is to use an online-tool.
I decided to use http://aes.online-domain-tools.com/.

Unfortunately this site requires the data to be in either base 256 or 16.
Seeing how the data is encrypted using AES it is likely not a good idea to represent in base 256, so I went with **16**.

I used this tool to convert from base-64 to hex: http://tomeko.net/online_tools/base64.php?lang=en.
