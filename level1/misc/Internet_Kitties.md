We were given a URL and a port. Combining these in the web-browser like this:
*shell2017.picoctf.com:53382*
we were given the web-page containing the flag.

Unfortunately it forwards us to an invalid page before we have a chance to copy it.
But using the *Network* -> *Response* debugging information in Firefox we can see the flag anyway.
