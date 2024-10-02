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
IF-ELSE 
- the if-else statement is a fundamental control structure that executes a block of code if a specified condition is true. i fcoondition is false, the else block is executed instead.
- structure : if block - executes whe the condition is true
- else if block - optional, executes another condition if previous one was false
- else block - executes when none of previous conditions were met
- if-else - statements are used when there are multiple conditions to evaluate. with diffrent outcomes depending on which conditions are true.

SWITCH STATEMENT 
- this is another control struture used for executing one block of code among many based on the value of an expression.
- switch keyword: evaluates an expression and matches it to one of several 'case' labels.
- case labels: each 'case' contains the code to to execute if the expression matches the label.
- break statemet: stops the execution of more cases after a match is found. without break, the code will continue executing the subsequent cases. 
-default case : executes if no matching case is found
- use case: the switch statement is ideal when you need to compare a single expression against multiple potential values.

































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








111

  <DOCTYPE html>
<html lang="en">
!
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Code Head's Hub</title>

    <style>
        body {
            margin-top: 200px;
            background-color: #1a3c35;
            font-family: Arial, sans-serif;
        }

        .container {
            padding: 1rem;
            max-width: 1300px;
            margin: 0 auto;
        }

        header {
            color: white;
            background-color: #1a3c35;
            align-items: center;
            position: fixed;
            width: 100%;
            top: 0;
            margin-bottom: 0;
            z-index: 20;
            background-color: #1a3c35;
            padding: 20px 0;
        }

        h2 {
            margin-left: 50px;
            font-size: 35px;
            margin-top: -10px;
            font-size: 20px;
          
        }

        nav {
            overflow: hidden;
            text-align: right;
            margin-top: -5px;
            margin-right: 60px;
            
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
            width: 2rem;
            height: 2rem;
            opacity: 0.5;
            border-radius: 1rem;
           margin-left: 1250px;
           
          
           
        }

        .imageR {
            width: 40rem;
            height: 26rem;
            background-color: #1a3c35;
            margin-bottom: 200px;
           
        }

        .home {
            display: flex;
            color: aliceblue;
            margin-top: -120px;
        }

        .container-left h1 {
            font-size: 2em;
            padding: 40px;
            margin-top: 60px;
            position: relative;
            top: 60px;
            left: 70px;
        }

        .container-left p {
            margin-left: 100px;
            line-height: 20px;
            font-size: larger;
        }

        .container-left {
            background-image: url('./image2.jpg');
            background-size: contain;
            width: 60rem;
            height: 44rem;
            background-repeat: no-repeat;
        }

        .container-right img {
            width: 44rem;
            height: 30rem;
            margin-top: 120px;
            opacity: 0.2;
        }

        .container-left button {
            background-color: white;
            color: #133a32;
            font-weight: bold;
            width: 236px;
            height: 60px;
            margin-left: 11rem;
            margin-top: 28px;
            font-size: large;
            border: none;
        }

        @media screen and (max-width: 800px) {
            .home {
                flex-direction: column;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="container">
             <a href="./indeex.html" ><img src="./profile-user.png" alt="profile-user" ></a> 
            <h2>CODE HEAD'S <br>HUB</h2>
            <nav>
                <a href="#home">HOME</a>
                <a href="#about-us">ABOUT US</a>
                <a href="#courses">COURSES</a>
                <a href="#book-us">BOOK US</a>
                <a href="#contact-us">CONTACT US</a>
              
            </nav>
        </div>
    </header>

    <section class="home" id="home">
        <div class="container-left">
            <h1>WELCOME TO THE<br>FUTURE OF<br>LEARNING: EXPLORE,<br>CREATE AND<br>INNOVATE.</h1>
            <p>LEARN WITH CONFIDENCE IN OUR SUPPORTIVE COMMUNITY!<br>EXPAND YOUR SKILLS, AND CONNECT WITH<br>A COMMUNITY
                THAT IS FUTURE-FOCUSED</p>
            <button><a href="#" style="color: #1a3c35;">START LEARNING</a></button>
        </div>

        <div class="container-right">
            <img class="imageR" src="./image 1.jpg" alt="Laptop Image">
        </div>
    </section>

    <section class="about-us" id="about-us">
        <!-- Content for About Us -->
    </section>

    <section class="courses" id="courses">
        <!-- Content for Courses -->
    </section>

    <section class="why-us">
        <!-- Content for Why Us -->
    </section>

    <section class="book-us" id="book-us">
        <!-- Content for Book Us -->
    </section>

    <section class="events">
        <!-- Content for Events -->
    </section>
</body>

</html>



222



    <!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Code Head's Hub</title>
  
  <style>
    body {
      margin-top: 200px;
      background-color: #1a3c35;
      font-family: Arial, sans-serif;
    }

    .container {
      padding: 1rem;
      max-width: 1300px;
      margin: 0 auto;
    }

    header {
      color: white;
      background-color: #1a3c35;
      align-items: center;
      position: fixed;
      width: 100%;
      top: 0;
      margin-bottom: 0;
      z-index: 20;
      background-color: #1a3c35;
      padding: 20px 0;
    }

    h2 {
     margin-left: 250px;
      font-size: 35px;
      margin-top: -40px;
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

    .imageR {
      width: 40rem;
      height: 26rem;
      background-color: #1a3c35;
      margin-bottom: 200px;
    }

    .home {
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

    .container-left p {
      margin-left: 145px;
      line-height: 20px;
      font-size: larger;
    }

    .container-left {
      background-image: url('./image2.jpg');
      background-size: contain;
      width: 60rem;
      height: 44rem;
      background-repeat: no-repeat;
    }

    .container-right img {
      width: 44rem;
      height: 30rem;
      margin-top: 120px;
      opacity: 0.2;
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

    @media screen and (max-width: 800px) {
      .home {
        flex-direction: column;
      }
    }
  </style>
</head>

<body>
  <header>
    <div class="container">
      <img src="./image3.jpg" alt="Logo" width="2rem" height="2rem">
      <h2>CODE HEAD'S HUB</h2>
      <nav>
        <a href="#home">HOME</a>
        <a href="#about-us">ABOUT US</a>
        <a href="#courses">COURSES</a>
        <a href="#book-us">BOOK US</a>
        <a href="#contact-us">CONTACT US</a>
      </nav>
    </div>
  </header>

  <section class="home" id="home">
    <div class="container-left">
      <h1>JOIN US WHERE<br>INNOVATION MEETS<br>INSPIRATION.</h1>
      <p>DIVE INTO CUTTING-EDGE TECHNOLOGY,<br>EXPAND YOUR SKILLS, AND CONNECT WITH<br>A COMMUNITY THAT IS FUTURE-FOCUSED</p>
      <button><a href="#" style="color: #1a3c35;">JOIN US</a></button>
    </div>

    <div class="container-right">
      <img class="imageR" src="./image 1.jpg" alt="Laptop Image">
    </div>
  </section>

  <section class="about-us" id="about-us">
    <!-- Content for About Us -->
  </section>

  <section class="courses" id="courses">
    <!-- Content for Courses -->
  </section>

  <section class="why-us">
    <!-- Content for Why Us -->
  </section>

  <section class="book-us" id="book-us">
    <!-- Content for Book Us -->
  </section>

  <section class="events">
    <!-- Content for Events -->
  </section>
</body>

</html>

rest api 
const http = require('http');
const fs = require('fs');

const port = 4000;
const dataFilePath = './items.json';

// Helper function to read data from JSON file
const readItems = () => {
  try {
    const data = fs.readFileSync(dataFilePath, 'utf-8');
    return JSON.parse(data || '[]');
  } catch (error) {
    console.error('Error reading items:', error);
    return [];
  }
};

// Helper function to write data to JSON file
const writeItems = (items) => {
  try {
    fs.writeFileSync(dataFilePath, JSON.stringify(items, null, 2), 'utf-8');
  } catch (error) {
    console.error('Error writing items:', error);
  }
};

const server = http.createServer((req, res) => {
  const url = req.url;
  const method = req.method;

  if (method === 'GET' && url === '/items') {
    // Read: Retrieve all items
    const items = readItems();
    res.writeHead(200, { 'Content-Type': 'application/json' });
    res.end(JSON.stringify(items));
  }

  else if (method === 'POST' && url === '/items') {
    // Create: Add a new item
    let body = '';
    req.on('data', chunk => {
      body += chunk.toString();
    });

    req.on('end', () => {
      const newItem = JSON.parse(body);
      const items = readItems();
      newItem.id = items.length ? items[items.length - 1].id + 1 : 1; // Auto-increment ID
      items.push(newItem);
      writeItems(items);
      res.writeHead(201, { 'Content-Type': 'application/json' });
      res.end(JSON.stringify(newItem));
    });
  }

  else if (method === 'PUT' && url.startsWith('/items/')) {
    // Update: Update an existing item by id
    const id = parseInt(url.split('/').pop());
    let body = '';
    req.on('data', chunk => {
      body += chunk.toString();
    });

    req.on('end', () => {
      const updatedItem = JSON.parse(body);
      const items = readItems();
      const index = items.findIndex(item => item.id === id);

      if (index !== -1) {
        items[index] = { ...items[index], ...updatedItem };
        writeItems(items);
        res.writeHead(200, { 'Content-Type': 'application/json' });
        res.end(JSON.stringify(items[index]));
      } else {
        res.writeHead(404, { 'Content-Type': 'application/json' });
        res.end(JSON.stringify({ error: 'Item not found' }));
      }
    });
  }

  else if (method === 'DELETE' && url.startsWith('/items/')) {
    // Delete: Remove an item by id
    const id = parseInt(url.split('/').pop());
    const items = readItems();
    const index = items.findIndex(item => item.id === id);

    if (index !== -1) {
      items.splice(index, 1);
      writeItems(items);
      res.writeHead(200, { 'Content-Type': 'application/json' });
      res.end(JSON.stringify({ message: 'Item deleted' }));
    } else {
      res.writeHead(404, { 'Content-Type': 'application/json' });
      res.end(JSON.stringify({ error: 'Item not found' }));
    }
  }

  else {
    // Handle unknown routes
    res.writeHead(404, { 'Content-Type': 'application/json' });
    res.end(JSON.stringify({ error: 'Route not found' }));
  }
});

server.listen(port, () => {
  console.log(`Server running on port ${port}`);
});



port
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Gcina's Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Gcina's Portfolio</h1>
            <nav>
                <ul>
                    <li><a href="#about">About Me</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="about" class="about-section">
        <div class="container">
            <h2>About Me</h2>
            <p>
                Hi, I'm Gcina, a passionate web developer specializing in full-stack development. I love crafting 
                responsive and dynamic web applications using the latest technologies. I aim to create clean, 
                efficient, and user-friendly code.
            </p>
        </div>
    </section>

    <section id="projects" class="projects-section">
        <div class="container">
            <h2>Projects</h2>
            <div class="project-grid">
                <div class="project-item">
                    <h3>Project 1</h3>
                    <p>A web app built with HTML, CSS, and JavaScript.</p>
                </div>
                <div class="project-item">
                    <h3>Project 2</h3>
                    <p>A full-stack application using Node.js and MongoDB.</p>
                </div>
                <div class="project-item">
                    <h3>Project 3</h3>
                    <p>A portfolio showcasing my design and development work.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="skills-section">
        <div class="container">
            <h2>Skills</h2>
            <ul class="skills-list">
                <li>HTML5</li>
                <li>CSS3</li>
                <li>JavaScript</li>
                <li>React.js</li>
                <li>Node.js</li>
                <li>Git & GitHub</li>
            </ul>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <div class="container">
            <h2>Contact</h2>
            <p>If you'd like to get in touch, feel free to reach out on any of the platforms below.</p>
            <ul class="contact-info">
                <li>Email: <a href="mailto:gcina@example.com">gcina@example.com</a></li>
                <li>LinkedIn: <a href="#">linkedin.com/in/gcina</a></li>
                <li>GitHub: <a href="#">github.com/gcina</a></li>
            </ul>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Gcina. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
/* Reset some default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
}

.container {
    width: 80%;
    margin: auto;
    overflow: hidden;
}

header {
    background: #333;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-size: 1.2em;
}

section {
    padding: 20px 0;
}

.about-section {
    background: #fff;
    padding: 50px 0;
    text-align: center;
}

.about-section h2 {
    margin-bottom: 20px;
}

.projects-section {
    background: #f4f4f4;
}

.projects-section .project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: 20px;
}

.project-item {
    background: #fff;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.skills-section {
    background: #fff;
    text-align: center;
}

.skills-list {
    list-style: none;
    margin-top: 20px;
    display: flex;
    justify-content: center;
}

.skills-list li {
    background: #333;
    color: #fff;
    padding: 10px 20px;
    margin: 0 10px;
    border-radius: 3px;
}

.contact-section {
    background: #f4f4f4;
    text-align: center;
}

.contact-section ul {
    list-style: none;
    margin-top: 20px;
}

.contact-section ul li {
    margin-bottom: 10px;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    margin-top: 20px;
}
rest api 

const http = require('http');
const url = require('url');
const PORT = 3000;
const CONTENT_TYPE_JSON = { "Content-Type": "application/json" };
const CONTENT_TYPE_HTML = { "Content-Type": "text/html" };
let products = [
    { id: 1, name: 'Product 1', price: 20.0 },
    { id: 2, name: 'Product 2', price: 30.0 },
  ];
 
const server = http.createServer((req, res) => {
 
    const parsedUrl = url.parse(req.url, true);
  
    if (req.method === 'GET') {
    
      handleGetRequest(req, res, parsedUrl);
    } else if (req.method === 'POST' && parsedUrl.path === '/product') {
      
      handlePostRequest(req, res);
    } else if (req.method === 'PUT' && parsedUrl.path.startsWith('/product/')) {
    
      handlePutRequest(req, res, parsedUrl);
    } else if (req.method === 'DELETE' && parsedUrl.path.startsWith('/product/')) {
  
      handleDeleteRequest(req, res, parsedUrl);
    } else {
     
      sendResponse(res, 404, CONTENT_TYPE_JSON, { error: 'Method not allowed' });
    }
  });
  server.listen(PORT, () => {
    console.log(`Product server listening on ${PORT}`);
  });
  const sendResponse = (res, statusCode, contentType, data) => {
    res.writeHead(statusCode, contentType);
    res.end(JSON.stringify(data));
  };
  const handleGetRequest = (req, res, parsedUrl) => {
    if (parsedUrl.path === '/') {
   
      sendResponse(res, 200, CONTENT_TYPE_HTML, `<b>Products <a href = '/product'>list</a> page</b>`);
    } else if (parsedUrl.path === '/product') {
     
      sendResponse(res, 200, CONTENT_TYPE_JSON, products);
    } else if (parsedUrl.path.startsWith("/product")) {
  
      const productId = parsedUrl.query.id || parseInt(parsedUrl.path.split('/').pop());
      const product = getProductById(productId);
  
      if (product) {
      
        sendResponse(res, 200, CONTENT_TYPE_JSON, product);
      } else {
        
        sendResponse(res, 404, CONTENT_TYPE_JSON, { error: 'Product not found' });
      }
    } else {
     
      sendResponse(res, 404, CONTENT_TYPE_JSON, { error: 'Endpoint not found' });
    }
  };
  
  
  const getProductById = (productId) => {
    return products.find(p => p.id === parseInt(productId));
  };
  const handlePostRequest = (req, res) => {
    let requestBody = '';
  
    req.on('data', (chunk) => {
      
      requestBody += chunk;
    });
  
    req.on('end', () => {
    
      const product = JSON.parse(requestBody);
      product.id = products.length + 1;
      products.push(product);

      sendResponse(res, 201, CONTENT_TYPE_JSON, product);
    });
  };
  const handlePutRequest = (req, res, parsedUrl) => {
    let requestBody = '';
  
    req.on('data', (chunk) => {

      requestBody += chunk;
    });
  
    req.on('end', () => {
     
      const updatedProduct = JSON.parse(requestBody);
      const productId = parseInt(parsedUrl.path.split('/').pop());
      const productIndex = products.findIndex(p => p.id === productId);
  
      if (productIndex !== -1) {
       
        products[productIndex] = { ...products[productIndex], ...updatedProduct, id: productId };
        sendResponse(res, 200, CONTENT_TYPE_JSON, products[productIndex]);
      } else {
       
        sendResponse(res, 404, CONTENT_TYPE_JSON, { error: 'Product not found' });
      }
    });
  };
  const handleDeleteRequest = (req, res, parsedUrl) => {
    const productId = parseInt(parsedUrl.path.split('/').pop());
    const productIndex = products.findIndex(p => p.id === productId);
  
    if (productIndex !== -1) {
     
      products.splice(productIndex, 1);
      sendResponse(res, 200, CONTENT_TYPE_JSON, { message: `Product with id ${productId} deleted successfully` });
    } else {
      sendResponse(res, 404, CONTENT_TYPE_JSON, { error: 'Product not found' });
    }
  };

