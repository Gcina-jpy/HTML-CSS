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
-  


CSS

- It is responsible for how everything looks
-the colors, fonts, and sizes. 





