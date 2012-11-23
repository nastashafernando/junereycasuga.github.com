---
layout: post
title: "Don't Get Fooled by W3Schools"
description: ""
category: Blogs
tags: [web development, junerey casuga, w3schools, w3fools]
---
{% include JB/setup %}

For years, I've been consulting W3Schools whenever I have to know more about HTML or Javascript. Numerous times, I’ve used them as reference thinking their content was credible.

I was wrong.

Recently, while doing research, I came across [W3Fools](http://w3fools.com) – a website made by the members of the Front-end Dev Community. While scrolling through the contents, I suddenly realized that the whole website was dedicated to exposing W3Schools as a "faculty source" of information regarding HTML and JavaScript.

Now, you might be wondering why W3Schools was deemed unreliable by W3Fools. Well, as it turned out, W3Schools was not in any way affiliated with [W3C(World Wide Web Consortium)](http://w3c.org) - an internation community that develops open standards to ensure the long-term growth of the Web. What's worse, W3Schools blatantly shows disregard for journalistic integrity by frequently publishing inaccurate content.

Here's a list highlighting some of the grossly misleadin content written by the people from W3Schools:


#### HTML

[www.w3schools.com/html5/html5_intro.asp](http://www.w3schools.com/html5/html5_intro.asp)

* W3Schools: The latest versions of Safari, Chrome, Firefox, and Opera support some HTML5 features. Internet Explorer 9 will support some HTML5 features.

* W3Fools: This is misleading. Many features that have existed for years in IE are just now being standardized by HTML5, e.g. `contenteditable`. IE8 also already supports `localStorage`, which is an HTML5 feature.

[www.w3schools.com/html/html_getstarted.asp](http://www.w3schools.com/html/html_getstarted.asp)

* W3Schools: [...] professional web developers often prefer HTML editors like FrontPage or Dreamweaver, instead of writing plain text.

* W3Fools: Professional web developers do not recommend the use of WYSIWYG editors.

[www.w3schools.com/html/html_frames.asp](http://www.w3schools.com/html/html_frames.asp)

* W3Fools: Again, frames are considered among the very worst of practices in modern Web development. In fact, they are considered so bad, they are no longer valid in HTML5.

[www.w3schools.com/html/html_getstarted.asp](http://www.w3schools.com/html/html_getstarted.asp)

* W3Schools: When you save an HTML file, you can use either the `.htm` or the `.html` file extension. We use `.htm` in our examples. It is a habit from the past, when the software only allowed three letters in file extensions. With new software it is perfectly safe to use `.html`

* W3Fools: Nitpicking to be sure, but Unix has supported arbitrary 255-character file names since 1983. That is hardly "new software", and illustrates the misunderstanding of basic principles of computing & software design that tends to permeate W3Schools material.
Extension are not necessary at all and if they are present they don't have to be `.htm` or `.html`. The key thing is that HTML files are served with the correct content-type e.g. `text/html`. (many web servers have some built in or preconfigured knowledge that `.htm` and `.html` should be served with the `text/html` content-type)

[www.w3schools.com/html/html_head.asp](http://www.w3schools.com/html/html_head.asp)

* W3Schools:

		<html>
			<head>Title of the document</head>
			<body>
				content of the document.....
			</body>
		</html>

* W3Fools: Their "minimum document example" is missing a DOCTYPE. It also differs from other "minimal document examples" on their site, such as the one on the HTML Introduction page, which is missing a `<head>` entirely.

[www.w3schools.com/tags/tag_hn.asp](http://www.w3schools.com/tags/tag_hn.asp)

* W3Schools: `<h1>` defines the largest heading and `<h6>` defines the smallest heading.

* W3Fools: This is not true. The heading element's number defines their rank for their importance on the page.


#### CSS

[www.w3schools.com/css3/css3_fonts.asp](http://www.w3schools.com/css3/css3_fonts.asp])

* W3Schools: Internet Explorer does not yet support the @font-face rule.

* W3Fools: This is wrong. In fact, Microsoft invented the `@font-face` at-rule.


#### JavaScript

[www.w3schools.com/JS/js_statements.asp](http://www.w3schools.com/JS/js_statements.asp)

* W3Schools: JavaScript code (or just JavaScript) is a sequence of JavaScript statements.

* W3Fools: Apparently declarations and expressions can go right to hell (since JavaScript only is a sequence of statements).


* W3Schools: Each statement is executed by the browser in the sequence they are written.

* W3Fools: This is not exactly true, either, as JavaScript [hoists](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Scope_Cheatsheet#Hoisting) variable and function declarations, meaning that those declarations are not defined in sequence.

[www.w3schools.com/jquery/tryit.asp?filename=tryjquery_ajax2](http://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_ajax2)

* W3Schools: `async: false`

* W3Fools: The first "A" in AJAX stands for "asynchronous" (or non-blocking). Promoting setting the `async` property to false when calling jQuery's [ajax](http://api.jquery.com/jQuery.ajax/) method without any context in an example that is likely to be copy/pasted around the net is grossly irresponsible.

[www.w3schools.com/js/js_functions.asp](http://www.w3schools.com/js/js_functions.asp)

* W3Schools: If you declare a variable within a function, the variable can only be accessed within that function. When you exit the function, the variable is destroyed.

* W3Fools: The whole concept of closures doesn't exist at W3Schools... Also, they never go over the difference between a function declaration and a function expression. I know this is for beginners, but they could at least put it in the advanced section, or make it apparent that functions are first-class?

[www.w3schools.com/js/js_loop_for.asp](www.w3schools.com/js/js_loop_for.asp)

* W3Schools: `for (var=startvalue;var<=endvalue;var=var+increment)`

* W3Fools: Not only do they forget about using the [`var`](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Statements/var) keyword to prevent the variable from leaking to the global scope, but you can't even use [`var`](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Statements/var) as variable name—it is a reserved word, and this code will generate a SyntaxError.

[www.w3schools.com/js/js_whereto.asp](http://www.w3schools.com/js/js_whereto.asp)

* W3Schools: Scripts in `<head>`

* W3Fools: In older browsers, placing scripts in the `<head>` has a negative impact on page performance. Until the script is done loading, resources below the script are blocked from downloading, and elements below the script are blocked from rendering. So try to put scripts at the bottom of the page, when possible.


What a revelation right? If you want to know some more unreliable content published by W3Schools, just [http://w3fools.com](http://w3fools.com).

As the good people at W3Fools say, "We believe W3Schools is harmful to the web. Web developers deserve better".

I wholeheartedly agree because I am one of them. I also believe that sharing bad information is toxic and can lead to more bad information being passed down to future generations of web developers.

The lesson her is obvious: Dont't believe everything you read. Even good doctors misdiagnose. Always ask and look for second or third opinions. Find sources that proved accurate, dependable information.

If you want to accelerate your education about web development, learn from the fine resources like [WebPlatform.org](http://webplatform.org/), [Opera Web Standards Curriculum](http://dev.opera.com/articles/view/1-introduction-to-the-web-standards-cur/#toc), [Google's HTML, CSS, and Javascript from the Ground Up](http://code.google.com/edu/submissions/html-css-javascript/), [SitePoint](http://reference.sitepoint.com/), and the [MDN (Mozzilla's Developer Network)](https://developer.mozilla.org/en-US/docs).

Also, if you want to contribute to the community, spread the word. Don't bee fooled, instead spread it the W3Fools way.