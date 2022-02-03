# Static HTML JS & CSS Blog Template

I wanted to create a simple web blog template using HTML, CSS and JavaScript on the browser side without using any server side programming (like PHP, node.js or Python), no hosting and no database.

Visual side is based on [fashion](https://www.myresponsee.com/fashion/) template from [Vision Design](https://www.visiondesign.sk).

Final result is available [here](https://arturwieczorek.github.io/static-blog-example/index.html).

This assumes one knows some Javascript, AJAX and can use JQuery.
This website uses static text files for content.

The most important features that needed to be added (as they won't be provided out of the box like in popular
blogging platforms and tools) are:


- pagination </br>
- search for posts </br>



<blockquote>
Store your blog article body content in text files using HTML. One for each article.
</br></br>
Post metadata is stored in local file database. I would recommend a JSON data format.
</blockquote>

Create list of objects in <b>blog_database.json</b> that represent blog posts where each
object contains information about post title, short summary and link to full article,
link to thumbnail image, date, author and other information that you would like to
include there e.g. catgegories, tags ...

Effectively the file serves as a database.


By accessing post objects you can retrieve articles data from the list for the
initial display. I used jQuery and pagination libraries for generating blog posts based on
posts objects data and Lunr.js for searching posts. Use popular browser tools to inspect
page code, files and console outputs.


Website can be hosted for free using GitHub Pages functionality.
Performance probably could be an issue with big objects full of data which will result in large local database file.
Otherwise it should be rather OK-ish.

I am not a front end developer and this was done as a fun project on the weekend.
Blog pages have the feature of navigation links to previous and next articles - this can also be implemented if needed.

My main goal was to display posts, add searching & pagination and it was implemented.

Another step could be to write a parser in Python (or other programming language) that will generate "database" file with JSON structure for all pages, articles based on directory contents. This might be an interesting small project and when putting more effort into it we could end up with a simple tool for creating static blog pages.
