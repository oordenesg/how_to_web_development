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

In this example, the *p* element is assigned an id of “top” and the *h1* element is assigned “bottom.” An id can be added to most elements on a webpage.
  
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

# Tables

When we create a web page, we can aggregate data to show trends or useful information. To do this, we must first add the tag *table*. This element will contain all of the tabular data we plan on displaying. After this, the second step is add rows using the table row element *tr*. Then, the third step is to add data points. To do this, we just need to use the *td* tag. Let's see and example:

```html
  <table>
    <tr>
    </tr>
    <tr>
      <td>Adam’s Greenworks</td>
      <td>14</td>
      <td>Package Items</td>
    </tr>
  </table>
```

To add titles to rows and columns, we can use the table heading element *th*. This tag has an attritube called *scope*  which can take the values *row* or *col*. Additionally to this, we can add more elements to our tables. A border could be added to a table using the *border* attribute and setting it equal to an integer. However, the vast majority of developers are using CSS to add style to HTML

```html
<table border="1">
  <tr>
    <th scope = "col">Company Name </th>
    <th scope = "col">Number of Items to Ship </th>
    <th scope = "col">Next Action </th>
  </tr>
  <tr>
    <td>Adam’s Greenworks</td>
    <td>14</td>
    <td>Package Items</td>
  </tr>
</table>
```

In HTML, we can also span columns using the *colspan* attribute. In the following example, we will see the data *Out of Town* spans the Monday and Tuesday table headings using the value 2 (two columns). The data Back in Town appear only under the Wednesday heading.

```html
<table>
  <tr>
    <th>Monday</th>
    <th>Tuesday</th>
    <th>Wednesday</th>
  </tr>
  <tr>
    <td colspan="2">Out of Town</td>
    <td>Back in Town</td>
  </tr>
</table>
```
Data can aslo span multiple rows using the rowspan attribute. The rowpsan attribute is used for data that spans multiple rows. With all these attributes, a table can grow to contain a lot of data and become unmanageable. When this happens, the table can be sectioned off so that it is easier to manage. Long tables can be sectioned off using the table body element *tbody*. The *tbody* element should contain all of the table’s data, excluding the table headings.


```html
<table>
  <tbody>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
    <tr>
      <th>Morning</th>
      <td rowspan="2">Work</td>
      <td rowspan="3">Relax</td>
    </tr>
    <tr>
     <th>Afternoon</th>
    </tr>
    <tr>
      <th>Evening</th>
      <td>Dinner</td>
    </tr>
  </tbody>
</table>
```

In the last example, we saw that the table’s headings were kept inside of the table’s body. We can also pu the table's headings off the table by using the tag *thead*. Addittionally to this, the bottom part of a table can also be sectioned off using thhe *tfoot* element. 


```html
<table>
  <thead>
    <tr>
      <th>Quarter</th>
      <th>Revenue</th>
      <th>Costs</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Q1</th>
      <td>$10M</td>
      <td>$7.5M</td>
    </tr>
    <tr>
      <th>Q2</th>
      <td>$12M</td>
      <td>$5M</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>Total</th>
      <td>$22M</td>
      <td>$12.5M</td>
    </tr>
  </tfoot>
</table>
```

Finally, we can use CSS to style tables. Tables, by default, are very bland. They have no borders, the font color is black, and the typeface is the same type used for other HTML elements.
```css
table, th, td {
  border: 1px solid black;
  font-family: Arial, sans-serif;
  text-align: center;
}
```
The code shows a demonstration of the various table aspects we can style using CSS properties

# Semantic HTML

Let's check semantics aspects of HTML to complement the structure of the web page. The traditional *header* tag can be replaced by using the *div* tag. However,  by using *header* tag our code becomes easier to read. When we use *header* the add a *nav* tag to defined a block of navigation links such as menus and tables of contents. Addittionally to this, there are two important structures called *main* and *footer*. These elements help describe here an element is located based on conventional web development standars.

The *main* tag is used to encapsulate the main content of our webpage. By using this tag instead of *div*, screen readers and web browsers are better able to identify tat whatever  is inside of the tag is the bulk of the content. On the other hand, the *footer* tag contains the contact information of our webpage.

```html
<!DOCTYPE html>
<html>
  <body>
    <header>
      <h1>Navigational Links</h1>
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#posts">Posts</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <p>This is where the main content will go once the page is built out!</p>
    </main>
    <footer>
      <p>Contact me at +1 234 567 8910 </p>
    </footer>
  </body>
</html>
```

There are two other elements that we can add in the body called *section* and *article*. The *section* tag defines elements in a document such as chapters, headings or any other are of the document with the same theme. The *artible* tag holds content that makes sense on itws own. This tag can hold content shuch as artibles, blogs, comments, etc. 

```html
<!DOCTYPE html>
<html>
  <body>
    <header>
      <h1>Navigational Links</h1>
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#posts">Posts</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    
    <main>
      <section>
        <article>
        <h2>Facts About Dogs</h2>
        <p>
        Dogs have a sense of time. It's been proven that they know the difference between a hour and five. If conditioned to, they can predict future events, such as regular walk times.
        </p>
        </article>
      </section>   
    </main>
    
    <footer>
      <p>Contact me at +1 234 567 8910 </p>
    </footer>
          
  </body>
</html>

```
In HTML, we can add content that is not required in order to understand the main structure. We can do this by adding the *aside* tag to mark additional information. This element can be used alongside other elements such as *article* or *section*. Some common uses of the *aside* element are for: Bibliographies, endnotes, comments or additional information.

What if we want to add an image or illustration? We can add *figure* and *figcaption* to do this. The *figure* is an element used to encapsulate media such as an image, illustration, diagram, code snippet, etc, which is referenced in the main flow of the document. On the other hand, the *figcaption* is an element used to describe an image. Usually, the *figcation* will go inside *figure*. We can also put another king of files on our website. The *audio* element is used to embed audio content into a document. Like *video*, *audios* uses the *src* attribute to link the source. Let's see an example.

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <header>
      <h1>Navigational Links</h1>
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#posts">Posts</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    
    <main>
      <section>
        <article>
          <h2>Facts About Dogs</h2>
          <p>
          Dogs have a sense of time. It's been proven that they know the difference between a hour and five. If conditioned to, they can predict future events, such as regular walk times.
          </p>
        </article>
        <aside>
          <p>A study was conducted on dogs being away from their owners for varying hours and the studies show that dogs who were away from their owners the longest showed the greatest amount of affection!
          </p> 
        </aside>
      </section> 
      <figure>
        <img src="https://content.codecademy.com/courses/SemanticHTML/dogimage.jpeg"/>
        <figcaption>A cute dog.</figcaption>
      </figure>  
      <audio controls>
        <source src="https://content.codecademy.com/courses/SemanticHTML/dogBarking.mp3" type="audio/mp3">
      </audio> 
  <!-- Create <video> and <embed> tag here -->
      <video src = "https://content.codecademy.com/courses/SemanticHTML/dog-video.mp4" controls>Video not supported
      </video>
      <embed src = "https://content.codecademy.com/courses/SemanticHTML/dog-on-beach.gif" />
      
    </main>
    <footer>
      <p>Contact me at +1 234 567 8910 </p>
    </footer>
  </body>
</html>
```

# Intro to CSS 

Previously we used HTML to create the main structure of our web page. However, the use of HTML can be visually unappealing on its own.  CSS is a languaghe web developers use to style the HTML content on web page. If we want to modify colors, font types, font sizes and more, CCSS is the tool for that job.

CSS has two different methods for writing code. The first sintax is what we called a *ruleset* while the second is what we called *inline*. Both have different components. Let's check all of them:

Ruleset Terms:
- Selector—The beginning of the ruleset used to target the element that will be styled.
- Declaration Block—The code in-between (and including) the curly braces ({ }) that contains the CSS declaration(s).
- Declaration—The group name for a property and value pair that applies a style to the selected element.
- Property—The first part of the declaration that signifies what visual characteristic of the element is to be modified.
- Value—The second part of the declaration that signifies the value of the property.

Inline Style Terms:
- Opening Tag—The start of an HTML element. This is the element that will be styled.
- Attribute—The style attribute is used to add CSS inline styles to an HTML element.
- Declaration—The group name for a property and value pair that applies a style to the selected element.
- Property—The first part of the declaration that signifies what visual characteristic of the element is to be modified.
- Value—The second part of the declaration that signifies the value of the property.

Let's see an example

![image](https://user-images.githubusercontent.com/76072249/119213344-66ee1980-ba8c-11eb-80f0-a1eef6697efd.png)

In we use the *inline* style, we can write the CSS within the HTML code. To do this we cann add the style attribute directly to the opening tag. After you add the attribute, you can set it equal to the CSS style(s) you’d like applied to that element.

```html
  <p style = 'color: green'>The world is full of fascinating places. Planning the perfect vacation involves packing up, leaving home, and experiencing something new.</p>
```

The problem with inline style is that if we want to style multiple *h1* elements. We would have to add inline style to each element manually. Fortunately, HTML allows us to write CSS code in its own dedicate secton wih a *style* element. To create an internal stylesheet, a *style* element must be added inside the of the *head* element. Afther adding the opening and closing *style* tags, we can begin writing CSS Code.

```html
<head>
  <style>
    p {
      color: red;
      font-size: 20px;
    }
  </style>
</head>
```

In real world, developers avoid mixing code by storing HTML and CSS in separate filex. We can do this by using the *.css* extension. When we have the HTML and CSS code in seperate files, they must be linked. To do this we can use the *link* element to link both files. This element must be placed within the head of the HTML file. The link element hast two attributes. The first, *href*, it must have the path of the CSS file. While, *rel* describes the relationship between the HTML and CSS file. Because we are linking to a stylesheet, the value should be set to *stylesheet*. If both files are stored in the same directory, then we can specifiy a relative path insted of  a URL. Let's seen an example.

```html
// Both the HTML and CSS code in a different path
<link href='https://www.codecademy.com/stylesheets/style.css' rel='stylesheet'>

// Both are in the same path
<link href='./style.css' rel='stylesheet'>
```
Let's check a new example.

```html
<head>
  <link href = "style.css" rel = "stylesheet" >
  <title>Vacation World</title>
</head>
```

## Selectors in CSS

In CSS, a selector is used to target the specific HTML element(s) to by styled. In this languaghe, the type selector matches the type element in the HTML document. Let's see the following example using the *p* tag.

```css
p {
  color: green;
}
```
We also use the universial selector to select all elements of any type. We can use this to reset default brower styling or to select all children of a parent element. The universal selector uses the * character in the same place where we specified the type selector.

```css
* { 
  font-family: Verdana;
}
```

As we know HTML elements can also have attributes. When we work with HTML and CSS a class attribute  is one of most common ways to select an element. Let's consider the following HTML. 

```html
<p class='brand'>Sole Shoe Company</p>
```
Here we have a class attribute with an opening tag *p*. This class attribute is equal to *brand*. To select this element using CSS, we can create a ruleset with a class selector of .brand.

```css
.brand {
}
```

Using the method, it is possible to add more than one class name to an HTML element's class attribute. Let's say there's a heading element that needs to be green and bold. We could write two CSS rulsets like:

```css
.green {
  color: green;
}
 
.bold {
  font-weight: bold;
}
```
After this, coudl include both of these classes one HTML element. Let's see how it works

```html
<h1 class='green bold'> ... </h1>
```

Oftentimes, we need to select just one element with CSS to give it its own unique style.  We can do this by using the *id* attribute. 

```html
<h1 id='large-title'> ... </h1>
```

Then, to select an element's ID with CSS, we prepend the *id* name with a number sign *#*. Let's see how to do this.

```css
#large-title {
 
}
```
As we saw in the HTML section, some HTML elements use attributes to add extra detail or functionality to the element. For instance, *href* and *src*.  The attribute selector can be used to target HTML elements that already contain attributes. Attributes can be selected similarly to types, classes and IDs. Let's see an exaple

```html
<img src='/images/seasons/cold/winter.jpg'>
<img src='/images/seasons/warm/summer.jpg'>
```

```css
img[src*='winter'] {
  height: 50px;
}
 
img[src*='summer'] {
  height: 100px;
}
```
    
In some cases it is possible to see that some elements can change after certain user interactions. For example, when we click on a blua link to visit to another page but when we return the link's text is purple. This is a common example of pseudo-class selector. In fact, *:focus* or *:disable* are all pseudo-classes. A pseudo-class is always written as a colon *:* followed by a name. Let's see an example.
    
```css
p:hover {
  background-color: lime;
}    
```
    
In CSS, classes are meant to be reaused over many elements. We can write CSS classes in a variaty of way by mixing classes. Let's think in the following situation. One headline needs to be bold and blue, and the other needs to be bold and green. Instead of writing separate CSS rules for each headline that repeat each other’s code, it’s better to write a .bold CSS rule, a .green CSS rule, and a .blue CSS rule. Then you can give one headline the bold green classes, and the other the bold blue classes.    
    
Browers need to decide the order in which CSS styles will by diplayed. A good practice in CSS in to style elements while using the lowest degree of specificity. IDs are the most specific selector in CSS followed by classes and finallytype. Let's see a example
    
```html
<h1 class='headline'>Breaking News</h1>
```
    
```css
h1 {
  color: red;
}
.headline {
  color: firebrick;
}
 ```
In the example code above, the color of the heading would be set to firebrick, as the class selector is more specific than the type selector. If an ID attribute (and selector) were added to the code above, the styles within the ID selector’s body would override all other styles for the heading.   
    
 In some cases, it is possible to require an HTML element to have two o more CSS selectors at the same time. This is done by combining multiple selectors, which we will refer to as chaining. 

```css
h1.special{
    } 
```

The code above would select only the *h1* elements with a class 'special'. However if a <p> element also had a class of special, the rule would not style the paragraph.
 
 In CSS we can also select elements that are nested within other HTML elements (descendants). For example, a list of elements. In we defined the attribute class of list as 'main-list' (for example). We can use the same method described previously to make sure that the list will appear in the context we expect. Let's see an example
    
```html
<ul class='main-list'>
  <li> ... </li>
  <li> ... </li>
  <li> ... </li>
</ul> 
```
```css
.main-list li {
}
```
    
Adding more than one tag, class, or ID to a CSS selector increases the specificity of the CSS selector. In CSS, it is possible to add CSS styles to multiple CSS selectors all at once. With this, we can prevent writing repetitive code. Let's see an example of repetitive code.
    
```css
h1 {
  font-family: Georgia;
}
.menu {
  font-family: Georgia;
}    
```
Insted of writing the same line font-family two times, we can separate the selectios by a comma to apply the same style to both. 
    
```css
h1, 
.menu {
  font-family: Georgia;
}
```

## Visual Rules
    
In CSS there are visual rules that we can use to style our website. One of the most common concepts is *Font* and it refers to the technical term typeface, or font family. To change this we can use the font-family property. There are two options:

```css
h1 {
  font-family: Garamond; // Option 1
  font-family: 'Courier New'; // Option 2 when the name of a typeface consists of more than one word
}
```
This is not the only way to customize the text. We also can modify the font size. To do this we can use the *font-size* property.

```css
p {
  font-size: 18px;
}
```` 
Another property is *font-weight* which controls how bold or thin text appears. Let's see an example.
    
```css
p {
  font-weight: bold;
}
```

In CSS our text always appears on the left side of the container in which it resides. To change this, we can use the *text*align* property and it will align text to the element that holds it. In this property we can set 4 values. These are: *left*,*center*,*right*,*justify*

 
```css
h1{
   text-align: right;
}     
```
In terms of colors, it's important to make two distinctions about this. Colors can affect the desing of the *Foreground color* or *Backgroud color*. The foreground color is the color that an elemnt appers. Conversely,  the brackground color refers to color behind the element.
 
 ```css
h1 {
  color: red; // foreground color
  background-color: blue;
} 
 ```
We can control the opacity as well. This is a measure of how to transparent an element is and it is measured from 0 to 1 (from fully invisible to fully visible).

```css
.overlay {
  opacity: 0.5;
}
```
Using CSS, we can change the background of an element. One option is to make the background of an element an image. This can be done by using the property *background-image*. We can use this property to use an image from a URL or folder.
  
 ```css
.main-banner {
  background-image: url('https://www.example.com/image.jpg'); // from a url
  background-image: url('images/mountains.jpg'); // from a folder
}
 ```
*!important* can be applied to specific declarations, instead of full rules. It will override any style no matter how specific it is. As a result, it should almost never be used. Once !important is used, it is very hard to override.
    
```css
p {
  color: blue !important;
}
 
.main p {
  color: red;
}
```
