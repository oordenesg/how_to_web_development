# how_to_web_development

In this repo I will add useful information to create a website. Here I have the fundamentals of HTML and CSS, the languages essential to developing websites. Additionally, I will add information how to set up a local web development environment.

First of all, it is important to describe the general process between the Internet and web browsers. The browser sends a request once the server recives the request. the server sends code and data as a response to the brower's request.  

What is a server? A server is a specialized computer connected to a network which provides resources or services. But, How do browsers and servers communicate? They use the internet protocol know as HTTP (hypertext transfer protocol) which allows for data transfer. There are 4 common HTTP requests:

1. GET: Used to retrieve information from given server
2. POST: used to send data to the server (like customer information or file upload)
3. PUT: used to replace current data with uploaded contetn
4. DELETE: removes current data. 

Another important concept is the HTTP status code. When a server responds to a client, the server indicates a status codes as a part of the response. These status codes indicate wheter or not the HTTP was sucessfully completed. If there was an error, these codes provide information regarding the error. The most common error is *404* code and it means that the requested resource was not found. 

So, in general, we can say that browers follow two main steps and this process different steps happen in a split second:

1. When we types in a URL, the server processes the request and sends the HTML file back to the client. The HTML files hold the content of a website and the links.
2. The browser will search the elements in the HTML and it will start to make additional HTML request for any other external resources. This process will consider the CSS stylesheets and the Javascrips files that make the webpage interactive. 
