---
title: HTML+CSS Basics
toc: show
---


# HTML+CSS Basics

The HTML+CSS Basics Workshop is a one-day introduction to creating web content. This class will focus on practical, technical skills with hands-on challenges and lots of time to practice and ask questions. Topics will include writing basic HTML and CSS, working with images and links, finding answers online, and using the development tools built into chrome.

Time 	| Unit
---		| ---
10:30	| Semantic Markup: How HTML and CSS work together
11:00	| HTML: Marking up a web page
12:15	| Documentation: How to find answers
*1:00*	| *Lunch*
1:45	| CSS: Styling a web page
3:00	| Using the Chrome developer tools
3:30	| Using Atom and Working Locally
4:00	| Links, Images, Paths
*5:15*	| *End of Class*


## Workshop Structure
- This workshop is divided into several parts. Each part begins with a brief introduction, followed by a hands-on exercise.
- If you get done early, keep exploring. If you don't get done, don't worry.
- At the end of each exercise we'll show and discuss an 'expert' solution.
- We will stick to the practical aspects; we won't get into the technical background.
- We will stick to the very high-level basics, focusing on how everything works together.
- A lot of important topics **won't** be covered: changing fonts, controlling box layout, etc.
- Fortunately, we **will** cover how to look that stuff up later.
- Inductive vs Inductive approach

## Semantic Markup: How HTML and CSS work together

### Learning Objectives
- What semantic markup is
- How HTML and CSS work together
- Practice identifying semantic structure of a document

### Overview
In documents, different words have different purposes. Some words form titles, some words form regular paragraphs, some are parts of lists. In web development these purposes are referred to as _semantics_. Often the semantic purpose of text informs how it should be styled. Title text is often bigger than paragraph text. Lists may be indented.

HTML and CSS are used together to explain the semantics of documents how they should look. HTML is used to describe the semantics of the document in a way that a web browser can understand. CSS is used to set style properties such as the font size and color to associate with different types of content.

If you want to make all the lists on a web page red, you need to use HTML to "mark up" where the lists are, and CSS to color them.

### More Information
- [Wikipedia: Semantic HTML](https://en.wikipedia.org/wiki/Semantic_HTML)
- [HTML5Doctor: Let's Talk about Semantics](http://html5doctor.com/lets-talk-about-semantics/)

### Challenge
[students (partners?) highlight content on printouts, label with semantic descriptions]
[one authentic material, one is what is coming up next]
[10 min]














## HTML: Marking up a web page

### Learning Objectives
- What HTML is
- HTML tag syntax
- Common HTML tags and semantic meaning
- Practice using HTML to mark up text documents


### Overview
HTML stands for HyperText Markup Language. It is used to provide information about the structure, organization, and purpose of content on a web page.

Properly marked up content can be understood by the web browser, allowing it to style the document way you want. Styles are defined in a separate language called CSS.

HTML 			| CSS 					| Javascript
---				| ---					| ---
Content			| Style					| Behavior
What it says	| What it looks like 	| What it does

#### HTML Syntax

Here is an example of a very basic HTML web page.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>HTML Basics</title>
	</head>
	<body>
		<h1>Hello, world.</h1>
        <p>This is a basic web page.</p>
		<img src="kitten.jpg">
	</body>
</html>
```

A few things to note in the above example:

- HTML uses tags (like `<h1>`) to mark up the purpose of text in a document.
- Most HTML tags work in pairs and surround the text they describe: `<h1>...</h1>`
- Opening tags look like this: `<h1>` and `<body>` and `<p>`
- Closing tags look like this: `</h1>` and `</body>` and `</p>`
- Tags can be nested: `<h1>` is  inside `<body>` and `<body>` is inside `<html>`
- Some tags, such as `<br>` and `<img>`, insert content into a page. Because these tags no not enclose content, they do not have a closing tag.

#### Important HTML Tags

Tag     | Purpose
---     |   ---
|
`html`  | wraps the entire document
`head`  | used to contain information that is not displayed on the web page
`title` | used to mark text that should be displayed in the document's tab (and bookmarks)
`body`  | used to mark the main content of the document
|
`h1`        | Headlines
`h2`..`h6`  | Less important headlines
`p`         | Paragraphs
`br`		| Creates a line break without starting a new paragraph (unpaired)
|
`ol`        | A numbered list
`ul`        | An unnumbered list
`li`        | An item in a list
|
`em`        | *emphasized text*
`strong`    | **strong text**
`code`      | `code text`
`blockquote`| Extended quotation
|
`a`			| creates a link
`img`		| inserts an image (unpaired)



### Important Note
In interesting feature of HTML is that browsers will try _very_ hard to show your document, even if there are mistakes in your HTML. In some ways this makes it easier to user and learn HTML: a simple mistake won't bring your whole page down. In other ways it makes it harder to learn and use: you don't get clear, immediate feedback when you make a mistake.

### More Information
- [Learn to Code HTML & CSS](http://learn.shayhowe.com/html-css/)
- [MDN: HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

### Challenge
- Open the "challenge" link below.
- Add HTML tags to mark up the semantic structure of the text.
- Try to make the rendered HTML match the "goal" link below.

[Challenge](https://jsbin.com/maronimafi/edit?html,output)
->
[Goal](challenges/challenge_html_solution.html)





## Documentation: How to find answers

### Learning Objectives
- Using Google to find technical information
- High-quality reference sites
- Practice finding information

### Overview
Webpages are built with three programming languages (HTML, CSS, and Javascript) and run on a variety of web browsers each with their own quirks. That is a lot of information to try to remember, and web technologies are constantly changing and growing. Finding technical answers online quickly is one of the most important skills required when making webpages.

Like any skill, you get better at searching for info when you practice.


### Tips for using Google for Technical Information
- Include the language in your search. `rounded corner` -> `rounded corner css`
- Include a reputable site in your search. `border properties` -> `border properties mdn`
- If the first few results are not what you are looking for, try a different search. `dotted line css` -> `dotted border css`
- Scan the first few results before you click.
- Look for titles that closely match what you are looking for.
- Look for sources that have been useful before.
- Don't forget that your browser can search for terms on a page: `command-f`
- Most common info can be found quickly. If you are not obviously on the right webpage for your answer, don't spend time on it. Go back to the search results and pick something else, or try rephrasing your search.
- Don't always use google. If you are looking for info on a particular HTML tag, CSS attribute, or JS function, a tool like devdocs.io might be better.


#### Good sources of info

Site | Description
--- | ---
[DevDocs](http://devdocs.io/)                   | Online reference application with info for *many* popular web technologies.
[Stack Overflow](http://stackoverflow.com/)     | Question and answer site with huge, well-curated database
[MDN](https://developer.mozilla.org/en-US/)     | Detailed, reliable technical documentation on HTML/CSS/Javascript and other web technologies.
[HTML5Rocks](https://www.html5rocks.com/en/)    | Tutorials and articles on specific aspects of HTML5
[CSSTricks](https://css-tricks.com/)            | Tutorials, quick reference, and other resources related to CSS


#### Challenge
- Answer the questions in the quiz linked below.
- This is an open-web quiz; you may use any website you like to find answers to the quiz questions.
- If you have extra time, spend some time reading up on topics included in the quiz.

[Finding Answers Quiz](https://goo.gl/forms/3N8oY4Vx0IPILUNK2)








## Lunch












## CSS: Styling a web page

### Learning Objectives
- What CSS is
- CSS rule-set syntax
- Common CSS properties
- Practice using CSS to style html documents


### Overview
CSS stands for Cascading Style Sheets. CSS is used to describe presentation styles for elements on a web page. CSS allows you to specify the size and color of text, borders, shadows, even the overall layout of the page.

HTML 			| CSS 					| Javascript
---				| ---					| ---
Content			| Style					| Behavior
What it says	| What it looks like 	| What it does

#### CSS Syntax

First, lets look at some css:

```html
h1 {
	font-size: 50px;
	color: red;
}

h2, h3 {
	font-size: 25px;
}

h3 {
	color: blue;
}
```

The example above has three **rulesets**. Lets look at the first one more closely:

```html
h1 {
	font-size: 50px;
	color: red;
}
```

This ruleset tells the browser to make all the `<h1>` elements on the webpage **big** and **red**. A few things to note about rulesets:

- Rulesets begin with a **selector**. The selector above is `h1`. This selector tells css that the following styles should be applied to any `h1` elements on the page.
- Rulesets may have more than one selector, separated with commas: `h1, h2`
- After the selector a pair of braces `{}` group two **declarations**.
- Declarations begin with a **property**: `color`;
- .. continue with a `:`
- .. followed by a **value**: `red`
- .. and end with `;`

#### Important CSS Properties

Tag     | Example Values 			| Purpose
---     |  ---						| ---
`color` 			| `red` `#00FF00` 	| Sets the font color
`background-color`	| `red` `#00FF00` 	| Sets the background color
|
`font-size`  		| `12px` `2em`		| Sets the size of the font
`font-weight`		| `bold` `normal`	| The font weight
`font-style`		| `italic` `normal` | Specify style variation of a font
`line-height`		| `1` `1.5`			| Spacing between lines of text
|
`padding`			| `5px` `1em`		| Extra space inside element
`margin`			| `5px` `1em`		| Extra space outside element
`margin-left`		| `5px` `1em`		| Just the left margin*

*`margin`, `padding`, `border` can be applied all the way around an element or just to the `-top`, `-right`, `-bottom`, or `-left`.

#### Inheritance
When a CSS property is applied to an element, it may be applied to the elements nested children as well. This is called **inheritance**.

In the following example, the color property will be applied to the `p` element. The `strong` element's text will also be red because the color property is inherited.

```
<p>This paragraph has a <strong>bold part</strong></p>
```
```
p { color: red; }
```

Not all CSS properties are inherited. You can check the [MDN CSS reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) to find out if a property is inherited.


#### Classes
Generally it good CSS practice to apply styles broadly. For example, you might make all `h1`s look a certain way. This leads to shorter, easier to understand CSS and more consistent visual design. In practice, however, you often need to get more specific. You might want a few `h1`s to be a different color for example.

You can use HTML and CSS together to create and style **classes**. Classes let you specify a specific set of elements.

```
<h1>Apples</h1>
<p>Apples are fruit.</p>

<h1 class="important">Bears</h1>
<p>Apples are animals.</p>

<h1>Cake</h1>
<p class="important">Cake is delicious.</p>
```
```
h1 {
	color: gray;
}
.important {
	color: pink;
}
```

- In the HTML, a class **attribute** was added to two tags in the HTML.
- In the CSS, a selector starting with `.` is used to apply a ruleset to elements marked with the `important` class.
- Use classes to describe the semantics of items in your document, not how you plan to style them.

#### Specificity

It is common that two rulesets will apply to the same element. In the example above, both the `h1` ruleset and the the `.important` ruleset apply to the "Bears" header. Since both rulesets set the `color` property, css must choose which property value to use. CSS gives priority to the more [specific](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Cascade_and_inheritance) selector's rule. CSS considers class selectors to be more specific than element selectors, so the `important` header ends up pink.

Understanding how CSS assigns priority is important as your projects grow more complex. Take a look at some of the linked resources for more detailed information.


### More Information
- [Learn to Code HTML & CSS](http://learn.shayhowe.com/html-css/)
- [MDN: CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

### Challenge

- Open the "challenge" link below.
- Add CSS rulesets to tell the browser how to style the html.
- Try to make the rendered HTML match the "goal" link below.
- You will need to CSS properties not listed above.
- You may alter the HTML if you like. For example, it may be helpful to add a `class` attribute to an element that requires special styling.

[Challenge](https://jsbin.com/zejuqukara/edit?html,css,output)
->
[Goal](challenges/challenge_css_solution.html)












## Using the Chrome development tools

### Learning Objectives
- What the Chrome Developer Tools are
- How to access and use the element inspector

### Overview
Chrome has a powerful set of built-in tools for web developers. Using these tools you can better understand how the browser interprets your HTML and CSS, see how long it takes to load each part of your page, and debug problems.

When working with HTML and CSS the Elements panel is very useful. This panel shows you which CSS rulesets the browser is using for each element. To inspect an element, you can right click on it and choose "Inspect" from the pop-up menu.

The left side of the Elements panel shows the structure of your HTML. The right side shows all the rulesets that are applied to the selected element. This view shows where each ruleset is defined and which properties are overridden by other rulesets.

You can even add temporary CSS declarations from the DevTools to quickly try out possible styles.

### More Information
- [Chrome DevTools Overview](https://developer.chrome.com/devtools)

### Challenge
- Answer the questions in the quiz linked below.
- Use the Chrome developer tools to explore the HTML and CSS of the sites mentioned in each question.
- If you have extra time, visit the New York Times website and use the DevTools to alter the headlines and style of the front page.

[DevTools Quiz](https://goo.gl/forms/4dq0j1krdbv1y9tC3)






## Using Atom and Working Locally

### Learning Objectives
- Install a text editor
- Creating a web page from scratch.
- Viewing a local web page in Chrome.

### Overview
Websites are made out of `.html`, `.css`, and `.js` files. While these are different languages, they are all based on simple text files meant to be written and read in a text editor.

There are many popular text editors, here are just a few:
- [Atom](https://atom.io/)
- [Sublime Text](https://www.sublimetext.com/)
- [VSCode](https://code.visualstudio.com/)

I use Atom for small web projects. I find the following Atom add-ons helpful:
- jsformat
- linter
- linter-jshint
- atom-live-server

### Local Server
You won't need to worry about local servers today, but you might by the end of the semester.

You can view simple HTML pages by simply opening them in a browser. As you begin to use more Javascript in your pages, you may find that this approach no longer works. This is because browsers impose restriction on what javascript can do from pages that are opened directly.

To work around these restrictions, it is common to use a local server. A local server is a program that works like a full-blown server, but runs on your local computer. Your web browser can connect to this local server and recieve files just as if they were hosted on a remote server.



### Challenge
Create a local web project.
- Create a folder on your computer to contain your project.
- Using a text editor, create an `index.html` file in that folder.
- Copy the HTML template below into your file.
- Open your `index.html` file in a browser.

```html
<!DOCTYPE html>
<html>
	<head>
		<title>Hello, HTML!</title>
	</head>
	<body>
		<h1>Hello, HTML!</h1>
        <p>This is a basic web page.</p>
	</body>
</html>
```



## Links, Images, Paths

### Learning Objectives
- How to create hyperlinks
- Linking to a CSS file
- How to embed images
- Understanding relative and absolute paths

### Overview
- How to create hyperlinks
- Linking to a CSS file
- How to embed images
- Understanding relative and absolute paths

### More Information

### Challenge
[students continue with the html created in previous challenge, adding styles, images, links to match provided goal part 2]
[30 min]






<style>
    .hljs-tag {
        color: #003399;
    }
    .hljs-name {
        color: #0033FF;
    }
    h2 {
        margin-top: 4em;
    }
</style>
