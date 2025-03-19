## Commit 1 Reflection
In this commit, the single-threaded HTTP server in rust is built by using only the TcpListener to 127.0.0.1:7878, then printing "Connection established!" whenever the browser is connected. I also used .unwrap() to skip over error checks just to get things working quickly, but it needs to be replaced with proper error handling before this could ever be reliable in a real application.

-----

## Commit 2 Reflection
![commit 2 screenshot](./commit2.png)
In this commit, an HTML page is returned and this is done by reading a hello.html file and including its contents in the HTTP response. The handle_connection function is also changed to load the file and build the response string. Other than that, the browser won’t render anything unless it receives a properly formatted HTTP response. This includes headers like Content-Length so it knows exactly how many bytes to read.