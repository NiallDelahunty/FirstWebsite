This is a personal website built to act as both a CV/resume as well as a reflection of my interests and experiences.
In this readme file I will outline exactly how my website has fit the specified requirements and explain where the
in my website I have placed those specific elements.

Section 1 - general requirements
(i) The website should have five pages including a homepage (index.html), a gallery page (e.g. page displaying images
multiple images in a structured format), and three pages of your own choice.

My website has five pages; a homepage (index.html), a gallery page ("gallery.html"), a hobbies page (hobbies.html),
a tutoring form page (tutoring.html) and a blog page (blog.html).

(ii) You should ensure that your HTML and CSS code is valid and should make appropriate use of HTML and CSS to separate
the content and presentation (styling) of the site.

All of the CSS styling is present in an external css file (style.css) and referenced to by each html page. The code for
all html pages and the css page has been run through the appropriate validators, with no errors.

Section 2 - specific requirements
1. Links to both your own pages and external webpages.
Links to internal pages are located in the <nav> tag (navigation bar buttons at the top of each page) at the start of each html page. The
same pages are linked under the heading 'sitemap' in the footer of the page.

External links are on all html pages located in the <footer> tag. Additionally on the email column, the text or image will open the default application
used for email, with my email address already in there. Here images for linkedin and github as well as the text links
below link to the associated websites. On the hobbies.html page, in the first '<div class = "fullwidthtext">', under the '<h2>climbing</h2>'
tag, in the <p> text the letters in blue 'free solo' link to an external website (youtube). On the same html page, under the '<h2> Reading </h2>'
tag, each of the images contained in the <h4> tags when clicked links to an external website (amazon).
On blog.html, under the '<div class="columntext">' in the <p> text the letters in blue 'Vitamin Sea' lilnk an external website (RTE).


2. A navigation bar
A navigation bar is present at the top of each html page, it is contained in the <nav> tag.

3. At least one table
A table is present in the tutor.html page, it is under the '<div class="table_container">' tag and is used to represent an availability timetable.

4.At least one list (ordered or unordered)
Ordered lists are present on every html page, as the navigation bar is a horizontal list. (<nav> tag). The <footer> tag of each html page consists of
4 unordered lists side by side. On tutor.html an unordered list is present under the <h2 id="subheading">Subjects</h2> tag and is used to list subjects.
An ordered list is present on the hobbies.html page under the surfing heading.

5. At least one local or embedded video
There are in total 4 embedded videos, 3 are located on the hobbies.html page under the '<h2>climbing</h2>', '<h2>surfing</h2>' and '<h2>hiking</h2>' tags.
The last one is on blog.html under the  '<h2>Wim hof method</h2>' tag. All use the embedded link provided by youtube '<iframe>'

6. At least four CSS3 and four HTML5 elements
HTML5: There are at least 4 HTML5 elements including: <nav>, <footer> and <figure> present on all html pages, <figcaption> is present on blog.html
CSS3: There are at least 4 CSS3 elements including: border-radius (index.html profile picture), justify-content, flexbox, animations (@keyframes) (tutor.html timetable)
and grid (hobbies.html-reading section)

7.Make use of the CSS positional properties (e.g. position, float):
Position is used for the text on the main figure in index.html (relative for the container and absolute for the text box)
Float is used on index.html to structure the main body to place the image and text containers beside each other as well as the images side by side
under 'career interests'.
Similarly float is used to place the main image side by side on hobbies.html, in tutor.html in the <form> section, to organise the form layout, and in the footer
of all html pages to organise the two footer containers beside each other and then to organise the contact detail lists side by side.

8.Make use of both inline and block elements

Both block and inline elements were used. Block elements such as <div>, <h1>-<h5>, <ol> , <form>, <section> and <hr> were used throughout all html pages.
The inline elements <span>, <br> and <em> were used.

Additional features of HTML and CSS3:
(a) Responsive text: I had the issue of the text associated with the background images on index.html and blog.html when sized down was remaining quite large while
the rest of the page got smaller (The main text also remained the same size but this was desirable as it was therefore still readable). I explored different ways of
making the text responsive, in the end the most suitable was to use the font-size: vw styling attribute which sets the text size to a % of the browser window.

(b) Enlarge figure when it is rolled over: In the blog.html page I had the issue of the figure information being slightly too small, as well as the figure legend being
unreadable at larger browser window sizes. To fix this I came across a styling technique to change the size of the container when the mouse is rolled over it. This can
be found on the css file as '.enlarge'. I included the figure legend (small text) in the same container as the image and set the background to white so that when the
image enlarged, you could not see the text it spread over.

(c) Responsive Gallery: My images were presented as individual squares. However I wanted the gallery to change based on how wide the browser window was, so that at its largest
there are 4 images across, and at its narrowest, they are lined up one by one. To do this the container they were in was displayed as a block with auto margins, the images
themselves were then floated to the left which meant that the as the browser window narrowed the number of images on each row changed.

(d)Grid/flex: I had a problem with my layout design. What had worked so well on the first index.html page (containers floated left and margins at auto with a fixed width) to make a responsive page
did not translate as well onto the hobbies.html page. Therefore I explored layout tools. Grid became an obvious choice given the range of things you can and do and the already grid like
appearance of the page. Under each of the hobby titles I placed the content into a 1 row, 1 column grid and set the grid-template-columns to auto. I fixed the width of the embedded videos
 to 100% of the column I was using so that there was maximum width on the video content. This allowed a neat, centered grid of text with accompanying video. In the reading section of hobbies.HTML
 I used another grid but this time with 2 columns and 3 rows. On blog.html in the section with the <h2>Wim hof method </h2> tag, display:flex was used instead and justify-content:center
 in order to achieve a similar appearance. Flex was also used in tutor.html to center the headings (tagged as <buttons> in the html) and the timetable. It is also used on blog.HTML
 to center the paragraph text (not the column text). Finally Flex is also used with justify-content:center to center the navigation bar.

(e)Animation: On tutor.html I wanted to have some way to emphasize the available times on the timetable (other than just colour). Therefore I looked into using animations. On the
CSS animation page on w3schools I found an animation which allowed me to transition from a grey background colour (all blocks of the timetable), to green (in only free times). I was
able to utilize the animation-delay and duration properties to allow sufficient time for the user to see it and the animation-fill-mode to keep the table in that colour pattern.
