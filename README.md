
**1. Introduction**

This is a personal website built to act as both a CV/resume as well as a reflection of my interests and experiences.
In this readme file I will outline exactly how my website has fit the specified requirements and explain where the
in my website I have placed those specific elements.

My website has five pages; a homepage (index.html), a gallery page ("gallery.html"), a hobbies page (hobbies.html),
a tutoring form page (tutoring.html) and a blog page (blog.html).

All of the CSS styling is present in an external css file (style.css) and referenced to by each html page. The code for
all html pages and the css page has been run through the appropriate validators, with no errors.

**Specific requirements**

  *Req1 - Links to both your own pages and external webpages.*

  *Req2 - A navigation bar*

  *Req3 - At least one table*

  *Req4 - At least one list (ordered or unordered)*

  *Req5 - At least one local or embedded video*

  *Req6 - At least four CSS3 and four HTML5 elements*

  *Req7 - Make use of the CSS positional properties (e.g. position, float)*

  *Req8 - Make use of both inline and block elements*


Additional features of HTML and CSS3:
-  Responsive text: I had the issue of the text associated with the background images on index.html and blog.html when sized down was remaining quite large while
the rest of the page got smaller (The main text also remained the same size but this was desirable as it was therefore still readable). I explored different ways of
making the text responsive, in the end the most suitable was to use the font-size: vw styling attribute which sets the text size to a % of the browser window.

- Enlarge figure when it is rolled over: In the blog.html page I had the issue of the figure information being slightly too small, as well as the figure legend being
unreadable at larger browser window sizes. To fix this I came across a styling technique to change the size of the container when the mouse is rolled over it. This can
be found on the css file as '.enlarge'. I included the figure legend (small text) in the same container as the image and set the background to white so that when the
image enlarged, you could not see the text it spread over.

- Responsive Gallery: My images were presented as individual squares. However I wanted the gallery to change based on how wide the browser window was, so that at its largest
there are 4 images across, and at its narrowest, they are lined up one by one. To do this the container they were in was displayed as a block with auto margins, the images
themselves were then floated to the left which meant that the as the browser window narrowed the number of images on each row changed.

- Grid/flex: I had a problem with my layout design. What had worked so well on the first index.html page (containers floated left and margins at auto with a fixed width) to make a responsive page
did not translate as well onto the hobbies.html page. Therefore I explored layout tools. Grid became an obvious choice given the range of things you can and do and the already grid like
appearance of the page. Under each of the hobby titles I placed the content into a 1 row, 1 column grid and set the grid-template-columns to auto. I fixed the width of the embedded videos
 to 100% of the column I was using so that there was maximum width on the video content. This allowed a neat, centered grid of text with accompanying video. In the reading section of hobbies.HTML
 I used another grid but this time with 2 columns and 3 rows. On blog.html in the section with the H2 tag, display:flex was used instead and justify-content:center
 in order to achieve a similar appearance. Flex was also used in tutor.html to center the headings (tagged as <buttons> in the html) and the timetable. It is also used on blog.HTML
 to center the paragraph text (not the column text). Finally Flex is also used with justify-content:center to center the navigation bar.

- Animation: On tutor.html I wanted to have some way to emphasize the available times on the timetable (other than just colour). Therefore I looked into using animations. On the
CSS animation page on w3schools I found an animation which allowed me to transition from a grey background colour (all blocks of the timetable), to green (in only free times). I was
able to utilize the animation-delay and duration properties to allow sufficient time for the user to see it and the animation-fill-mode to keep the table in that colour pattern.
