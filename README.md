# HTML-CSS

html 

-HTML forms the foundation of website and web app development. 
-allows you to make sure your content is understandable to both people and computers.
-HTML is a language used to structure web pages.
-It uses tags, which are enclosed in less-than and greater-than symbols, to mark different elements.

FOR EXAMPLE: <P>This is a paragrap</p> 

<p> - being the opening tag
"This is a paragraph " - being content 
</p> - being the closing tag 

- These tags work together to define elements.which are like packages containing content.
- the purpose of an html markup is to give meaning to the content and help computers understand

- theres also nested hlml emlements 

FOR EXAMPLE :  <p>this is a paragraph that has <em>emphasized text</em> for effect </p>
- <em></em> being the nested tag 



-an entire HTML document is basically a bunch of HTML elements nested inside each other

FOR EXAMPLE : <article> 
              <h1>head</h1>
              <p>paragraph ONE</p>
              <p>paragraph TWO</p>
              <p>paragraph THREE has <em>emphasized text</em></P>
              </article>
this structure tells that article has one headline 3 paragraphs with third having emphasized text.  

NOTE H1 AND P TAGS ARE NESTED IN ARTICLE ELEMENT !

HTML HEADLINES : 
-usually web pages contain various titles,headlines and sub headings .
- when dealing with lengthly text, these elements serve the purpose of dividing content into smaller chunks.
- -they help people comprehend stucture of page.
- headlines can be found anywhere in a page .
- there are 6 difrrent html elements used for marking up headlines.( h1 to h6).
-  h1 being the largest and most and h6 smallest .

HTML BOLD AND ITALICS
- there are 4 html elements for these 2 for italics and 2 for bold.
  FOR ITALICS
- . We use the "<i>" element to apply visual italics and the "<em>" element to add emphasis.
- note that <i> and <em> tag might look identical but they are for diffrent purposes and carry diffrent meanings. 
  FOR BOLD
- The first one is the "<strong>" element, which is used to show importance, seriousness, or urgency.(This element adds meaning to the text)
- <b>" element is more generic and neutral. (this element does not carry any sort of meaning)
- you can use <b> element if you want to catch readers attention or you want to make a phrase bold without conveying meaning.
  
HTML LISTS
-  In HTML there are 3 types of lists.
- the ordered list  <ol>
                                  <li> </li>
                                  <li>  </li>
                                  </ol> 
-  unordered list(grocery list)<ul>
                    <li> milk </li>
                     <li> eggs </li>

                   </ul>
-   definition lists
  


ARIA Roles
-ARIA Roles are like extra attributes that we can add to HTML elements to make them more meaningful and help browsers understand what they represent. 
-ARIA (Accessible Rich Internet Applications) roles are attributes used in HTML to enhance accessibility for people with disabilities. They help screen readers and other assistive technologies understand the purpose and function of various elements on a webpage.

Formatting HTML
-  HTML does not pay much attention to spaces, tabs, or line breaks
-  but there are exeptions
-  If you use elements like <pre>, <code>, or <textarea>, or if you modify the whitespace handling with CSS, then extra spaces and indentations can matter.

FOR EXAMLE : <p>this is    an   example   of   putting  extra spaces 
   but browser will ignore </p>


HTML COMMENTS : 
-You enhance code readability by adding comments that explain its purpose.
you can add a comment by inserting "<!--" at the start of comment and "-->" at the end of comment 
FOR EXAMPLE : <!-- this is a comment -->

Unusual Characters : 
- Instead of using a regular space, we can use a special kind of space called a non-breaking space in HTML.
-  you can use "&nbsp;"ensuring they stay on the same line
  FOR EXAMPLE: <p> my Name is gcina &nbsp;&nbsp;</p>

HTML Navigation and Linking
- When we want to create a link, we use the A element, which stands for anchor. To do this, we need to add an href attribute with a URL enclosed in quotes.
- this URL is where the link take us.
-href stands for Hypertext Reference

FOR EXAMPLE:  < a href="https//:example.com">This is a link</a>
for adding and image <a href ="https//:example2.com"><img src="https//:example.com/imagefile"></a>

HTML URL PATHWAYS 
-URL (Uniform Resource Locator): It’s the address used to access resources on the web. It usually consists of several parts:

Protocol: How data is transferred (e.g., `http`, `https`).
Domain: The main part of the address (e.g., `example.com`).
Path: The specific location or file on the server (e.g.,`folder/page.html` /).

FOR EXAMPLE: <a href="https://example.com/folder/page.html">Link</a>

- Same Directory:
`page.html`: Refers to a file in the same directory as the current document.
FOR EXAMPLE: <a href="about.html">About Us</a>

Subdirectory:
`folder/page.html`: Refers to a file in a subdirectory called folder.
FOR EXAMPLE: <a href="images/photo.jpg">View Photo</a>

Parent Directory:
`../page.html`: Refers to a file in the parent directory. The ".." moves up one directory level.
FOR EXAMPLE: <a href="../contact.html">Contact</a>

Navigation : 
- Creating a navbar in HTML is a common task for building a website. A navbar typically includes links to different sections or pages of a website.
  THIS IS HOW TO CREATE A NAVBAR :
  <nav role="navigation"arial-label="mainmenue">
  <ul class="navbar">
  <li><a href="#menue">menue</a></li>
  <li><a href="#about"></a></li>
  <li><a href="#contact"></a></li>
    
  </ul>
<</nav>

IMAGES 
- When we want to add an image to a webpage, we use the image element, which is simply written as IMG.
FOR EXAMPLE:
            img src="image.jpg" alt="brown dog" width="400" height="300">
  
-irst, we have the source attribute (SRC), which tells the browser which image file to load. 
-Then we have the alt attribute (ALT), which provides a text description of the image. 
-Lastly, we have the width and height attributes, which determine the size of the image.

-There are four main file formats commonly used on the web these days, each with its own strengths and weaknesses when it comes to compressing images. 
-GIFs are great for compressing illustrations that have large areas of the same color
-SVGs are perfect for logos, icons, and other types of illustrations.
-JPGs are a popular choice for compressing photographs.
-PNG is a newer format that works well when you need transparency in a photograph.

for image captions 

<figure> <img src="https://figuresource.com/40289/alfonso.jpg" width="720" height="354" alt="The Gracious Host" > <figcaption> Alfonso serving pancakes </figcaption> </figure>

WORKING WITH AUDIO
- The audio element is diffrent from image, it has both opening and closing tags (making it more mordern giving it more power and flexibility)
- just like the image element we use a source attribute to provide URL OF The audio file
FOR EXAMPLE: <audio controls>
             <source src="path/to/your-audio-file.mp3" type="audio/mpeg">
              Your browser does not support the audio element.
    </audio>
    
WORKING WITH VIDEO
- Just like working with audio To display a video, use the source attribute to specify the video file. And if the controls attribute is added,
 the browser will automatically create a video player.
- The controls attribute adds video controls, like play, pause, and volume.

- It is a good idea to always include width and height attributes. If height and width are not set, the page might flicker while the video loads.

- The <source> element allows you to specify alternative video files which the browser may choose from. The browser will use the first recognized format.

- The text between the <video> and </video> tags will only be displayed in browsers that do not support the <video> element.

Working With Captions and Subtitles
- We are going to use the track element and link it to a text file to add captions to the video. This element adds functionality to the video player, allowing viewers to toggle captions on and off or switch between different subtitle options.

    FOR EXAMPLE : <video width="200px" height="100px" controls src="enter location of the video">
             <track src="https://freetestdata.com/wp-content/uploads/2022/02/Free_Test_Data_1MB_MP4.mp4"
             kind="captions"
             label="english"
             srclang="en">  
</video>          

Embedding Media via Iframes
-   Embedding refers to taking content from one site and placing it within the middle of another site's page.
-   There is a wide range of content that can be embedded on a page. For instance, a map from Google
  
HTML Content Identification
- The lang attribute is used to specify the language of a webpage. If the whole page is in one language, Set the language on the main element that wraps everything else.
- If your webpage has multiple languages, specify the language for each part of the content.
- 

HTML Page
- Firstly, the file should begin with a doctype statement
- when we including this one, we are saying, "Hey, this is a modern web page, so follow modern best practices and treat it accordingly."
- we enclose everything else on the page within an HTML element
- Declare the language being used and the content flow direction
- The head contains all the metadata that the browser needs to know but will not display on the page. The body, on the other hand, is for all the content and is composed of various elements already discussed in this course. The body is where most of the action happens.
- the declearation of doc type statement,HTML element, head and body are building blocks of every website.

  Working with Forms and Interactive Elements
-  A user could type anything in there, even though one of them is supposed to be for an email field. That is because we have yet to tell the browser what type of input is required from these fields.
-  you can fix this by adding the type attribute to each input. for the name field, indicate the type equals text.
- for the email field, tell the browser to collect an email address, and help user fill in the right info by trype being equals to email.
- also tell browser that our button is a submit button.
- we can also add a required attribute making email required
- lastly we include the placeholder (suggestions of what should go in the field)
- we can also add the value attribute.
  
FOR EXAMPLE : <section class="sign-up">
              <form action="example.html" method="get">
              <label for="name">Name</label>
              <input name="name" id="name" type="text">
              <label for="email">email</label>
              <input name="email" id="email" type="email" required 
               placeholder="m@example.com">
              <button>sign-up</button>
             </form>
              </section>

HTML Tables
- you can use tables for diffrent reasons, comparing prices of things that are for sale, population data by town election results e.t.c
-To create an HTML table, you use several different HTML elements in just the right combination. Table, TR, TH, and TD.
-the table element wraps around the whole table, around all our content and markup for that table, marking the beginning and end of the table itself.
- TR element stands for table row and wraps
- TH element stand for table header and defines a header for a column
- TD element stands for table data and mark up the cells of data 






CSS

- It is responsible for how everything looks
-the colors, fonts, and sizes.
- what if we want to make a specific paragraph green? Or maybe we just want to make a portion of a paragraph green? How is this done?
  You can assign classes to HTML elements to create a reference point for styling. A class is an attribute that can be added to any HTML element, providing additional details about that element.

  Advanced CSS properties 
- you can change the color/ style html and css links
- first start by using "a" which is an anchor, which you will use as refrence when styling.
- One common exception is the "a:hover" state, which triggers when we hover over a link.
- you can use text decoration as none to remove the under line under links
- Now, when you hover over the links, they change color and the underline disappears. This was not possible before without the hover style. If we remove the hover style, nothing happens when you hover over the links.
- Define the nice blue color as the "a:link" style for unvisited links, and the lovely shade of purple (785ef0) as the "a:visited" style for visited links.
- 
Debugging CSS with Borders and Background Colors
-Sometimes you come across a problem when styling elements with CSS. You might wonder which element you should style or why your styles are not working as expected.
  - When facing such challenges, debugging can be very helpful.
  - one trick to use is to change background color or have a border to the element you wnat to style
  - like "border: 2px solid red."
  - this will reveal hidden information and this will show where exactly the element
 

  jAVASCRIPT 
- javascript is a programmiing language used to make a web page interactive

variables- the container that holds data values 
data types - the type of data that the variable holds 

we have several data types like arrays,numbers,booleans,string,object 
- you cam declare a variable using var,let and const 

let - can be reassigned 
const- cannot be re assigned 

for example : let name = "Gcina";  the name can be reassigned.  
              const age = 23; age cannot be re-assigned or changed.
 OPERATORS : - are symbols or keywords used to perform operations on values 
we have diffrent types of operators : 

1- arithmetic operators- these are used for mathematical calculations ( multiplication* +;-;% and exponential **) FOR EXAMPLE : let a = 5 + 6; 

2- assignment operators - used to assign values to variables ( assign , += , -=, *=,/=)
FOR EXAMPLE: let x = 10; or x/=4  // x= x/4

3- comparison operators - used to compare values and return booleans [ equal;!(not equal); ===(strict equal); !==(strict not equal) ; >; <; >=(greater or equal to), <=(less than or equal to).FOR EXAMPLE :  5 !='6'

4- logical operators: used to combine multiple conditions [&&(AND);||(OR); !(NOT).]
FOR EXAMPLE : true&& false // false
              true||false // true
              !true // false 

5-Unary operations : operate on a single operand [ ++(increment/add) ; --(decrement), typeof (data type)
FOR EXAMPLE : let x = 5; 
              x++;   //6 

             let y = 6 ; 
             njabulo++


6- ternary operations : a shorthand for an if-else statement (condition ? expression1 : expression2 ) 
FOR EXAMPLE : let k = (2 < 4 ) ?'yes': 'no';


TYPES OF EXPRESSIONS: 
1- arithmetic expression: these use arithmetic operators to perform calculations. 
                         FOR EXAMPLE : let price = price * quantity;
                         
2- comparison expressions : use comparison operators to evaluate condition. 
                          FOR EXAMPLE: let isAdult = age >= 18; 

3- logical expressions : combine multiple condition using logical operators 
                       FOR EXAMPLE : let canVote = (age >= 18) && (citizen === true) 
                          
CONTROL STRUCTURES (if-else, switch)
- 


<!DOCTYPE html>
<html lang="en-US" dir="ltr">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Code Head's Hub</title>
  <link rel="stylesheet" href="">
  <meta name="description" content="">
  <meta name="keywords" content="">


</head>

<body>
  <style>
    body{
      margin-top: 200px;
      background-color: #1a3c35;
      
    }
    .container {
      padding: 1rem;
      max-width: 1300px;
      margin: 0px auto;
    }

    header {
      color: white;
      background-color:#1a3c35;
      align-items: center;
      position: fixed;
      width: 100%;
      top: 0;
      margin-bottom: 0;
      z-index: 10;
      background-color: #0f2722;

    }


    h2 {
      text-align: center;
      font-size: 35px;
      margin-top: -70px;
    }

    nav {

      overflow: hidden;
      text-align: right;
      margin-top: -5px;
    
     

    }

    nav a {
      color: white;
      font-weight: bold;
      text-decoration: none;
      padding: 1rem 1.25rem;
      
      

    }

    nav a:hover {
      background-color: aliceblue;
      color: #1a3c35;
    }

    .container img {
      width: 4rem;
      height: 4rem;
      opacity: 0.5;
      border-radius: 2rem;

    }

    
    


    .imageR{
      width: 40rem;
      height: 26rem;
      background-color: #1a3c35;
      margin-bottom: 200px;
      

      
 
    }
    .home{
      display: flex;
      color: aliceblue;
      margin-top: -120px;
  
    }
    .container-left h1 {
      font-size: 2em;
      padding: 30px;
      margin-top: 60px;
      position: relative;
      top: 60px;
      left: 120px;
     

    }

    .container-left p{
     margin-left: 145px;
     line-height: 20px;
     font-size: larger;
    }
   
     

  
   .container-left{
      background-image:   url(./background.png);
      background-size: contain;
      width: 60rem;
      height: 44rem;
      background-repeat: no-repeat;
     

    }
    
    .container-right img{
      width: 44rem;
      height: 30rem;
      margin-top: 120px;
    }

    .container-left button {
      background-color: white;
      color: #133a32;
      font-weight: bold;
      width: 236px;
      height: 60px;
      margin-left: 15rem;
      margin-top: 135px;
      font-size: large;
      border: none;
    }
  

    @media screen and (max-width:800px) {

      .home{
        flex-direction:column;
    }
    
      
    }

    
  </style>


  <!-----This is  top black box on our website-->
  <header>



    <div class="container">
      <img src="./image (3).png" width="2rem" height="2rem">

      <h2>CODE HEAD'S HUB</h2>
      <nav>
        <a href="#home">HOME</a>
        <a href="#about-us">ABOUT US</a>
        <a href="#courses">COURSES</a>
        <a href="#book-us">BOOK US</a>
        <a href="#contact-us">CONTACT US</a>

      </nav>
    </div>

    <!-----Logo-->


    <!-----navigation bar-->


    <!-----This is  top black box on our website-->



    <!-----This is  top black box on our website-->

  </header>




  <!-----This is where the main content of our website will go-->
  <main>

    <!-----home section  ( landing page of our website)-->

    <section class="home">
      <div  class="container-left">
          <h1>JOIN US WHERE<br>  INNOVATION MEETS <br>INSPIRATION.</h1>
          <p>DIVE INTO CUTTING-EDGE TECHNOLOGY,<br>EXPAND YOUR SKILLS,AND CONNECT WITH A <br>COMMUNITY THE FUTURE FOWARDS</p>
          <button><a href="" >JOIN US></a></button>
     
      </div>

      
      <div class="container-right">
        <img class="imageR" src="./laptop.png" >
      </div>

       

    </section>



    <!-----About section  ( company mission & vision )-->
    <section class="about-us">

    </section>


    <!-----Courses section  ( this is where we will list all of our available courses)-->
    <section class="courses">

    </section>


    <!-----Why us section  ( telling our client why they should choose us )-->
    <section class="why-us">

    </section>



    <!-----book us section  (this where our clients will book sessions with us )-->
    <section class="book-us">

    </section>

    <!-----Events section  ( this is where we will list all of available events  internally )-->
    <section class="events">


    </section>




  </main>




  <!-----This is the bottom green box of our website including all company info and additional content not less important-->
  <footer>


  </footer>


</body>

</html>
