# Use UT library proxy to access journal articles off campus

UT library provides a proxy server so that we can directly see e-journals.  

URL of the proxy server is `ezproxy.lib.utexas.edu`.  

### How to use proxy
The simplest way to use the proxy is adding proxy URL to the journal website URL you want to access.  
  
For instance, in order to see Nature (www.nature.com), you can use this URL: `www.nature.com.ezproxy.lib.utexas.edu`.  
For the first time in a session, you will be asked your EID and password.
  
It can work for any pages of individual articles as well.  
Just put `.ezproxy.lib.utexas.edu` after original server name.
  
`http://science.sciencemag.org/content/early/2016/05/04/science.aaf0899`  
 will be accessible via  
`http://science.sciencemag.org.ezproxy.lib.utexas.edu/content/early/2016/05/04/science.aaf0899`  

### Bookmark button to apply proxy
I even do not want to remember and type the sequence.  
Then I set up a bookmark on my browser like "Reload Button" which we used to use at UMD,
so that I just click the button at any article page (see [UMD library website](http://lib.guides.umd.edu/reload-button) for more info).  
  
Following is the java script you can set to a bookmark.  
This script automatically inserts the proxy server url after the host name.  
  
```javascript
 javascript:(function() {var u=window.location.toString(); var
 n=u.search('[^/]/[^/]');
 window.location=u.substring(0,n+1)+'.ezproxy.lib.utexas.edu'+u.substring(n+1);})()
````
  
Unfortunately proxy server in UT seems not as smart as one in UMD.  That is, if
your query is not on the list of proxy server, it will give you just
an Error page, instead of passing back to the original page.
