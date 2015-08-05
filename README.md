xkcd_slim
=========

**xkcd_slim** is a Single-page Application ([SPA]) that displays an slim version
of any given **[xkcd]** comic.

## Purpose

I intended to write an [SPA] to display the title, image and alternative text of
the **[xkcd]** comic specified by a parameter. It should provide navigation
buttons to go to the previous and next comic so you would read the comics
chronologically one after another.


### Why not use the xkcd web site?

* You need to put the mouse over the image to read the alternative text and wait
  (precious seconds wasted here).
* Loads more stuff than what you need just to read the comic.


### There are a few xkcd viewers out there. Why does the world need another one?

I wanted (a761783) to start a project to apply a couple of things I've
learned about web apps development. I also wanted to find out what else I still
din't know and learn it. Here is the list of things I've discovered:

* Same origin policy ([SOP])
* Cross-origin resource sharing ([CORS])
* Cross-site ajax requests are possible if the web server supports CORS and
  accepts your request.
* There are a few ways to overcome the cross-site ajax request limitation if the
  web server is not under your control ([1], [2]).
* You can use [YQL] to get the DOM of any HTML document converted into JSON.



[SPA]: https://en.wikipedia.org/wiki/Single-page_application
[xkcd]: http://xkcd.com/
[SOP]: http://en.wikipedia.org/wiki/Same_origin_policy
[CORS]: https://en.wikipedia.org/wiki/Cross-origin_resource_sharing
[YQL]: https://developer.yahoo.com/yql/
[1]: http://jquery-howto.blogspot.com/2013/09/jquery-cross-domain-ajax-request.html
[2]: http://stackoverflow.com/a/17299796/684403
