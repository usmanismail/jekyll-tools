jekyll-tools
============

A set of scripts to automate some common jekyll tasks

Create_Post
-----------
This scripts uses a template to generate a new jekyll post for you using the the provided template. The usage is as follows:
	
	create_post.rb title author categories tags. 
	
* If the title has spaces use inverted commas to make sure its treated as a single parameter, the spaces will be converted into dashes when generating the file name (and hence post url) for your post. Any other characters that are not allowed as *nix filenames should be avoided.

* My blog has multiple authors and so I have added the author tag to the template you can skip this if you have a single author blog. 

* categories and tags are both comma separated lists of phrases which will be used as categories and tags for your post respectively. If there are spaces in a category or tag then encase the whole list in quotation marks. 

The default template looks like this, the TITLE, DATE, AUTHOR, CATEGORIES and TAGS keywords will be replaced by the script.  

    layout: post
    title: TITLE
    date: DATE
    author: AUTHOR
    categories: 
    - CATEGORIES
    tags:
    - TAGS

This code is based on code from Calus Witt which can be found [here](http://clauswitt.com/A-Simple-Create-New-Blogpost-Script.html)
    