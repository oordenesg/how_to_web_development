# how_to_web_development

# Introduction to Web development

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

## What is HTML 

HTML is the skeleton of all web pages. It provides structure to the content on a website considering text, images, videos and more. 

In HTML, we write the content in a similar way to how we would write it in any essay.We would start from the title and then we would continue with the content of our essay until we reached the conclusion.

In HTML we separete content and annotation by using HTML tags which are denoted by angle brackets *<>*. Let's see and example

```html
<p> Hellow World!</p>
```
In this example, we called *element* the entire line. The first *<p>* is called opening tag followed by the content and closing tag. However, in HTML there are different tags. Let's see the following example. 
  
```html
<h1>Jetsetter Travel Agency</h1> 
<p>With over 25 years of experience in concierge, high-end travel planning, we'll provide you with the highest quality services. Every vacation is unique, custom, and tailored to your tastes.</p>
<button>Click here!</button>
```

In this example we've added the *h1*, *p* and *buttom* tag. Using *h1* we can add titles or headings while using *p* we can add text. We additionally add a button on our website. 

In HTML, we can link our text to other text. This is what we called hypertext and it means that the text expands beyond the traditional constraints of the written word. Instead of reading documents from beginning to end, like you would read a book, someone going through hypertext can browse. By clicking on links from one document to another, the user can navigate to whatever page they find the most interesting and carve their own unique path through the web.

```html
<a> href = "www.learnhowtocode.com" > Learn to code </a>
```
The example above shows that when we click the text of this link they will be directed to the website *learnhowtocode.com*

## What is CSS? 

CSS is a languague that can provide style to the content of an HTML page. This includes colors, fonts, positioning, layout, and more. When we work with CSS, we could recognize many of the HTML tags. The good thing is that CSS contains selectors that specify the HTML elements to which the style should be applied as well as visual rules that specify how that content should be displayed. 

# Introduction to HTML

## Structure

As we said previously, HTML is the skeleton of all web pages and is core to front-end development work. This is language is the first step in creating websites. In this section we will focuse on how to add and modify basic content on a page.

One key HTML elements we used to build a webpage is the *body* element. Only the content inside the body tags is going to be displayed. To add these tags we just need to add
```html
<body>
  <p>What's up, doc?</p>
</body>
```
HTML is organized as a tree of relationships. In the previous example we added a *body* tag and the *p* tag. When an element is contained inside another element, it is considered as a child of that element. We can also say that the child element is nested inside the parent element. Let's see a more complicated example.

```html
<body>
  <div>
    <h1>Sibling to p, but also grandchild of body</h1>
    <p>Sibling to h1, but also grandchild of body</p>
  </div>
</body>
```
In this structure, the *body* element is the parent of *div*. The *h1* and *p* elements are children of *div* and siblings of the *body* element.

## Headins in HTML

In HTML there are six different headings and they can be usd for a variety of purposes. The main header is *h1* and the relevance of the headings decreases as the number increases. For this reason the least important header is *h6*.

```html
<body>
  <h1>The Brown Bear</h1>
  <h2>About Brown Bears</h2>
  <h3>Species</h3>
  <h3>Features</h3>
  <h2>Habitat</h2>
  <h3>Countries with Large Brown Bear Populations.</h3> 
  <h3>Countries with Small Brown Bear Populations.</h3>
  <h2>Media</h2>
</body>
```
