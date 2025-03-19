## Commit 1 Reflection
In this commit, the single-threaded HTTP server in rust is built by using only the TcpListener to 127.0.0.1:7878, then printing "Connection established!" whenever the browser is connected. I also used .unwrap() to skip over error checks just to get things working quickly, but it needs to be replaced with proper error handling before this could ever be reliable in a real application.

