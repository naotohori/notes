UT library provides a proxy server so that we can directly see
e-journals.  URL of the proxy server is `ezproxy.lib.utexas.edu`.  For
instance, in order to access to Nature (www.nature.com), you can use
this URL: `www.nature.com.ezproxy.lib.utexas.edu`

It can work for any pages of individual articles as well.  Just try to
add `.ezproxy.lib.utexas.edu` after original server name.
`http://science.sciencemag.org/content/early/2016/05/04/science.aaf0899`
 will be accessible via
`http://science.sciencemag.org.ezproxy.lib.utexas.edu/content/early/2016/05/04/science.aaf0899`


 I even do not want to remember and type the sequence.  Then I set up a
 bookmark on my browser like "Reload Button" we used to use at UMD, so
 that I just click the button at any article page.  (Please see
 http://lib.guides.umd.edu/reload-button for more info.)

 Following is the java script you can set to a bookmark.  This script
 automatically inserts the proxy server url after the host name.

```javascript
 javascript:(function() {var u=window.location.toString(); var
 n=u.search('[^/]/[^/]');
 window.location=u.substring(0,n+1)+'.ezproxy.lib.utexas.edu'+u.substring(n+1);})()
````

 Unfortunately UT's server seems not as smart as UMD's.  That is, if
 your query is not on the list of proxy server, it will give you just
 an Error page, instead of passing back to the original page.

