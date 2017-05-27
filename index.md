Do you ever wonder what happens when you type a URL into a browser or how the browser loads the webpage you had requested? 
If not, let’s take a trip down the browser lane now & find out what’s happening behind the scenes, shall we?

### Type URL in browser
The web page address (e.g. www.google.com) that you type into a browser is called an URL (Uniform Resource Locator). Every URL or simply, a web address has a unique IP (Internet Protocol) address associated with it. An IP address is a series of numbers (e.g. http://74.125.224.72/ ) which uniquely identifies every system on the Internet. It’s like how phone numbers in a phone book would translate to a person’s name. So instead of remembering the numbers directly, we just type in the website’s URL and the browser fetches the respective IP address and thereby its contents for us. 

### DNS Lookup
But the browser by itself does not automatically know each and every IP address on the Internet. It looks it up with the help of DNS (Domain Naming Servers), which is indeed like a phone book. They maintain a directory of domain names and translates them to IP addresses.

### TCP Connection
After looking up the IP address, the browser then contacts and establishes a TCP connection with the server located at that IP address. Transmission Control Protocol (TCP) is a set of rules that defines how to establish and maintain these network connections.

### HTTP GET Request
Then the browser sends a HTTP (GET) request to the server, which is a request to load the desired webpage. 

This whole process is again like making a phone call, where in you look up a person’s number, dial it, wait for the connection to be made and then when someone says “hello” on the other end, you start the conversation.

### Server handles the HTTP request
The server on the other end at the specific IP address then handles the request made from the browsers by a special software running on them known as web servers, e.g. Apache, IIS, etc. 

### Server launches the handler plug-in
The web server then passes on the request to the proper request handler which is a program written to handle web services e.g. PHP, .NET, Python, etc.

### Server generates HTTP response
Then this request-handling program generates a HTTP response and sends it back to the browser.

### Browser receives the HTTP response & displays web page content
The browser now receives the HTTP response and parses it.
Rendering of this response on the browser is also done in phases – first the bare bone HTML structure of a web page is rendered and then multiple GET requests are sent to fetch each new resource on the page like images, style sheets, JavaScript files, etc. which is a repetition of the above mentioned process. And now once all the required information is fetched, the browser displays the web page we see on the screen. Voila!

Though this all seems to be a lot time consuming, this isn’t as bad as it seems. It all happens with in split seconds and the web page gets rendered in no time☺

This is only a bird’s-eye view of the client-server page rendering process. Hope you enjoyed it and feel free to dive deep in and explore. All you have to do is type in your search @ google.com and press enter but I bet this time you will have a better clue of what happens between pressing Enter and your search results being displayed ☺
