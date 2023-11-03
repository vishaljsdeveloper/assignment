a. What is the main functionality of the browser? 

 

After hitting the URL, the first thing that needs to happen is to resolve IP address associated with the domain name. DNS helps in resolving this. DNS is like a phone book and helps us to provide the IP address that is associated with the domain name just like our phone book gives a mobile number which is associated with the person’s name. 

 

youtube.com 
Browser 
DNS 
199.223.232.0 
 

After getting an IP address, resolver stores it in its cache so that next time, 

if the same query comes then it does not have to go to all these steps again. 

It can now provide IP address from their cache. 

This is all about the steps that is followed to resolve IP address that is 

associated with the domain name. 

Browser 
ycnnut:e com 
Resolver 
Seach Atrh«itative 
Root Server 
TLD server 
Authoritative Name 
Server 
 

 

 

c. Rendering engine and its use. 

 

Rendering Engine: As the name suggests, this component is responsible for rendering a specific web page requested by the user on their screen. It interprets HTML and XML documents along with images that are styled or formatted using CSS, and a final layout is generated, which is displayed on the user interface. 

 

 

font-family : 
Padding: 50px 
Font-size; gpt; 
display: none 
CSSOM 
DOM 
font-family ; Arial 
Padding : 
Render Tree 
ont4ize: Opt: 
 

 

A web browser is a software application that enables a user to access and display web pages or other online content through its graphical user interface. Refer to the image below to understand the key components involved in building a  web browser. 

 

 

UI Backend 
Networking 
User Interface 
Browser engine 
Rendering engine 
JavaScript 
Interpreter 
 

d. Parsers (HTML, CSS, etc) 

 

 

We type a URL and press the enter and the server responds with index.html. However, an HTML content is not what we see when we visit a website... we see a web page with colors and backgrounds and animations and pictures. So there's a process that turns the HTML content to a pretty webpage, and that is parsing and rendering! 

 

 

 

httpş MşaurabMaware _ in 
I • m Satxath Dawye 
 

 

 

High Level Components of a browser. 

 

The user interface: this includes the address bar, back/forward button, bookmarking menu, etc. Every part of the browser display except the window where you see the requested page. 

The browser engine: marshals actions between the UI and the rendering engine. 

 

The rendering engine : responsible for displaying requested content. For example if the requested content is HTML, the rendering engine parses HTML and CSS, and displays the parsed content on the screen. 

Networking: for network calls such as HTTP requests, using different implementations for different platform behind a platform-independent interface. 

 

User Interface 
Browser Engine 
8 
Rendering Engine 
 

 

UI backend: used for drawing basic widgets like combo boxes and windows. This backend exposes a generic interface that is not platform specific. Underneath it uses operating system user interface methods. 

JavaScript interpreter. Used to parse and execute JavaScript code. 

Data storage. This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem. 

 

e. Script Processors 

 

 

The script processor parses each incoming document’s JSON source fields into a set of maps, lists, and primitives. To access these fields with a Painless script, use the map access operator: ctx. 

 

 

POST _ Ingest/plpellne/_slmulate 
"pipeline": { 
"processors": 
"script" 
"description": "Extract 'tags ' 
"lang": "painless" 
"source": """ 
from 'env' field", 
String[] envSp1it = ctx[ 'env' 'delimiter']); 
ArrayList tags = 
new ArrayList(); 
tags . ' position ' . trim( ; 
ctx[ 'tags'] = tags; 
"params" 
"delimiter": " % 
"position" : 
1 
"docs": 
source 
"env": " 
esel-prod" 
 

 

 

The script processor executes Javascript code to process an event. The processor usesapure 

Go implementation of ECMAScript 5.1 and has no external dependencies. This can be useful in 

situations where one of the other processors doesn't provide the functionality you need to filter 

events. 

The processor can be configured by embedding Javascript in your configuration file or by 

pointing the processor at external file(s). 

 

f. Order of script processing 

 

 

1. Before business rules: Scripts configured less than 1000. 

2. Before engines. The following are not We'd like your help! 

 3. Before business rules: Scripts configured greater than or 

equal to 1000. Powered by 

4. The data base operation (insert, update, delete). 

5. After business rules: Scripts configured to execute after the database operation with an order less than 1000. 

6. After engines. The following are not executed in any specific order: 

 7. Email notifications. The following are executed based on the weight of the notification record: 

  8. After business rules (Only active records). Scripts configured to execute after the database operation with an order greater than or equal to 1000. 

 

 

 

 

 

g. Layout and Painting 

  

 

•layout refers to the process of constructing a render-tree and using that tree to compute the 

exact position and size of each object 

painting refers to the process of taking the previously computed positions drawing the colors 

to the screen 

 

Layout: Calculates the size and position of each 

elements on a Web page is relative, which means a single element can affect others. For example, in case element to be displayed on the screen. The layout of there is a change in the width of the element, the widths of its child and grandchild elements get affected. 

Therefore, the layout process often gets involved for the browser. 

Paint: Essentially, painting is the process of filling in pixels. It requires painting of text, colors, images, 

borders, shadows, and other visual effects of a DOM element. In general, the painting gets completed in 

multiple layers. 

 


 

 

Layout has a notion of three-dimensions (z-indexes), structure (lines, boxes, flow) and parent-child relationships (trees). In painting, we flatten all of this information down to two-dimensions. The result of a paint is justa2d-grid of pixels and their colors. It's what you see on the screen. All structure has been lost. 

 