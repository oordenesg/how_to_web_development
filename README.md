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

## Divs

One of most importan elements in HTML is the *div* element. This element means "division" and divies the page into sections. There sections are very useful for grouping elements together. These sections could hav same styles for all the HTML elements inside. We can also style the *div* element a as whole. These *div* elements could contain any text or other HTML elements like text, images or videos.

```html
<body>
  <h1>The Brown Bear</h1>
  <div>
    <h2>About Brown Bears</h2>
    <h3>Species</h3>
    <h3>Features</h3>
  </div>
  <div>
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <h3>Countries with Small Brown Bear Populations</h3>
  </div>
  <div>
    <h2>Media</h2>
  </div>
</body>
```

## Attributes

If we want to expand an element's tag, we can do so using an attribute. These attributes are content added to the opening tag of an element and can be used in several ways from providing information to changing styling. in HTML, attributes are made up of two parts: Name of the attribute and value of the attribute. The following code block shows an example.

```html
<div id="intro">
  <h1>Introduction</h1>
</div>
```
One the most common attribute is the id. We can use it to specify content and is really helpful when we use an element more than once. The main objective of *id* is that it allows us to identify content. Let's see another example.

```html
<body>
  <h1>The Brown Bear</h1>
  <div id ="introduction">
    <h2>About Brown Bears</h2>
    <h3>Species</h3>
    <h3>Features</h3>
  </div>
  <div id = "habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <h3>Countries with Small Brown Bear Populations</h3>
  </div>
  <div id = "Media">
    <h2>Media</h2>
  </div>
</body>
```

## Displaying Text

When we want to display text in HTML we can use a *paragraph* or *span* denoted by *p*.

```html
<body>
  <h1>The Brown Bear</h1>
  <div id="introduction">
    <h2>About Brown Bears</h2>
        <p>The brown bear (Ursus arctos) is native to parts of northern Eurasia and North America. Its conservation status is currently Least Concern. There are many subspecies within the brown bear species, including the Atlas bear and the Himalayan brown bear.</p>
    <h3>Species</h3>
    <h3>Features</h3>
        <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id= "media">
    <h2>Media</h2>
  </div>
</body>
```

We can also style text using HTML tags. To do this we can use *em* to emphasize text or *strong* to highlights importan text. Additionally, we can also add a line break element within our HTML code. We can do this by adding an opening tag *br* in our code. In this cases, it is necessary a closing tag.

```html
<body>
  <h1>The Brown Bear</h1>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br><br> There are many subspecies within the brown bear species, including the Atlas bear and the Himalayan brown bear.</p>
    <h3>Species</h3>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
  </div>
</body>
```

In our text, we can also add list of elements. To do this we can use an unordered list tag *ul* to create a list of item in **no particular order** with a bullet point. The <ul> element should not hold raw text and won’t automatically format raw text into an unordered list of items. Individual list items must be added to the unordered list using the <li> tag. The <li> or list item tag is used to describe an item in a list. Let's see an example:
  
```html
<ul>
  <li>Limes</li>
  <li>Tortillas</li>
  <li>Chicken</li>
</ul>
```

We can also add ordered list in out HTML code. Instead of using *ul* we just need to add *ol*. Let's see an example using *ul* and *ol*.

```html
<body>
  <h1>The Brown Bear</h1>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the Atlas bear and the Himalayan brown bear.</p>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
      <ol>
        <li>Russia</li>
        <li>United States</li>
        <li>Canada</li>
      </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
  </div>
</body>
```

## Images

The *img* tag allows us to add images to a our web pages. This tag requires both opening and closing tag. However, the end of tag should by followeb by slash */*. Th *img* tag requires a attribute called *src*. The src attribute must be set to the image’s source, or the location of the image. In this case, the value of *src* must be the URL of the image. Let's see example

```html
 <div id="media">
    <h2>Media</h2>
      <img src = "https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg"/>
  </div>
```
Addittionally to the *src* attribute, there is another attribute called *alt* which means alternative text. We can use this attribute when we need to add the meaning to the images on our sites. In general, the value of alt should be a description of the image.

```html
 <div id="media">
    <h2>Media</h2>
    <img src="https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg" alt="brown bear face" />
  </div>
```

## Videos

In addition to images, HTML also supports displaying videos. Like the *img* tag, the *video* tag requires a src attribute with a link to the video source. Unlike the *img* tag however, the *video* element requires an opening and a closing tag.

```html
<div id="media">
    <h2>Media</h2>
    <img src="https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg" alt="A Brown Bear"/>
    <video src = "https://content.codecademy.com/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" width="320" height="240" controls>Video not supported</video>
  </div>
```

# Preparing for HTML

All HTML files require certain elements to set up the document correctly. We can let web browsers know that we are using HTML by starting our document with a document type declaration. To do this we need to declare *!DOCTYPE html* and  it must be the first line of code in our HTML document. This declaration tells the browser what type of document to expect, along with what version of HTML is being used in the document.

In general we can say that this declaration provides two pieces of information:
1. The type of document
2. The HTML version to expect

To create HTML structure and add content, we must add opening and closing *html* tags after *DOCTYPE html*. Let's see and example

```html
<!DOCTYPE html>
<html>
</html>
```
In some cases, it is necessary to add information about the page. This information must no be displayed directly on the web page. To do this, we need to add the *head* element after *html* tag and before the *body* tag. This element will contain the metadata for a web page. The metadata is information about the page itself

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Coding Journal</title>
  </head>
</html>
```
If we were to open a file containing the HTML code in the example above, the browser would display the words My Coding Journal in the title bar (or in the tab’s title). Let's see an example graphically. The site title will be title inside the *head* tag.

![image](https://user-images.githubusercontent.com/76072249/118415911-01a8bb80-b67b-11eb-87d0-4645a4d22842.png)

## Linking to Other Web Pages

We can add links to our web page by using the opening and closing tag *a* called anchor. This tag has an attribute called href which is the URL. Let's see the structure of this tag.

```html
<a href="https://www.wikipedia.org/">This Is A Link To Wikipedia</a>
```
When we click on a URL, we expect a new window to open. To do this, we need to add a new attribute called *target*. For a link to open in a new window, the target attribute requires a value of *_blank*. The target attribute can be added directly to the opening tag of the anchor element, just like the href attribute. 

```html
<a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">The Brown Bear</a>
```
Having explained how to add external links to our website, a new question could arise is how to add more pages to our website. First of all, when making multi-page static websites, web developers often store HTML files in the root directory, or a main folder where all the files. 

```cmd
project-folder/
|—— about.html
|—— contact.html
|—— index.html
```
In projects, HTML files ares often stored in the same folder.  If the browser is currently displaying index.html, it also knows that about.html and contact.html are in the same folder.

```html
  <body>
    <a href = "./index.html"> Brown Bear</a>
    <a href = "./aboutme.html">About Me</a>
    <h1>The Brown Bear</h1>
```

Additionally, HTMLL allows us to turn nearly any element into a link by wrapping that element with an *anchor* element. Using this technique we can turn images into links by wrapping the *img* element with an *a* element.

```html
<a href="https://en.wikipedia.org/wiki/Opuntia" target="_blank"><img src="https://www.Prickly_Pear_Closeup.jpg" alt="A red prickly pear fruit"/></a>
````
## Linking to Same Page

When we create a web page we must be sure that our code is descriptive. To do this we can add an *id* to our elements in our web page.

```html
<p id="top">This is the top of the page!</p>
<h1 id="bottom">This is the bottom! </h1>
```

In this example, the <p> element is assigned an id of “top” and the <h1> element is assigned “bottom.” An id can be added to most elements on a webpage.
  
```html
<!DOCTYPE html>
<html>
<head>
  <title>Brown Bears</title>
</head>

<body>
  <a href="./index.html">Brown Bear</a>
  <a href="./aboutme.html">About Me</a>
  <h1>The Brown Bear</h1>
    <ul>
      <li><a href = "#introduction">Introduction</a></li>
      <li><a href = "#habitat">Habitat</a></li>
      <li><a href = "#media"> Media</a></li>
    </ul>
  <div id="introduction">
    <h2>About Brown Bears</h2>
    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the
      Atlas bear and the Himalayan brown bear.</p>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">Learn More</a>
    <h3>Species</h3>
    <ul>
      <li>Arctos</li>
      <li>Collarus</li>
      <li>Horribilis</li>
      <li>Nelsoni (extinct)</li>
    </ul>
    <h3>Features</h3>
    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>
  </div>
  <div id="habitat">
    <h2>Habitat</h2>
    <h3>Countries with Large Brown Bear Populations</h3>
    <ol>
      <li>Russia</li>
      <li>United States</li>
      <li>Canada</li>
    </ol>
    <h3>Countries with Small Brown Bear Populations</h3>
    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>
  </div>
  <div id="media">
    <h2>Media</h2>
    <a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank"><img src="https://content.codecademy.com/courses/web-101/web101-image_brownbear.jpg"/></a>
    <video src="https://content.codecademy.com/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" height="240" width="320" controls>Video not supported</video>
  </div>
</body>

</html>
```
