### Writing HTML

If you look at the left side of the screen within **Atom** you'll see our file, *index.html* listed. Double click on it, and we'll begin writing our first **HTML** code.

**HTML** is the basic building block of the internet. It represents the code which has been used to display every website you've ever visited. At it's core, it is a system used to mark different elements for your browser to display them in specific ways.

Read the following code and carefully type it into the *index.html* file.

<div class="filename">index.html</div>
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Epicodus Workshop Project</title>
  </head>
  <body>
    <h1>My Programming Goals</h1>
  </body>
</html>
```

Here we've used several different element types. As you can see, each elements opens (example: `<html>`) and then closes (example: `</html>`). These are called **tags**. The `/` within the closing tag is what differentiates them.

* `<html>` tells the browser that everything within it is HTML.
* `<head>` the head efines information about the webpage that will not be displayed, but is important (more on this later).
* `<body>` contains the information to be displayed to the user.
* `<h1>` is a header tag. There are headers 1-6, and they correspond to different text sizes.

Let's save (`command/alt + S`), and then open our webpage. In the Terminal, enter the command `open index.html`.

Now we can see our page.

<hr>

### Expanding HTML

Let's add some more impressive elements to our HTML.

Lets start with another header. Follow along and match your HTML to the following code snippet. Note that we're limited the snippet to the `<body>` element alone for now.

<div class="filename">index.html</div>
```html
...
  <body>
    <h1>My Programming Goals</h1>
    <p>Every journey is easier if you <strong>know where you're going.</strong> <em>-unknown</em></p>
  </body>
...
```

* The `<p>` element is a paragraph. This is the basic text element used in HTML, and is used to display most basic text to the user.

Save the file, and refresh the page in your browser. Note that the `<strong>` and `<em>` tags within the paragraph element have made some changes to how the text appears. Can you figure out what they do?

Let's use a new element to display an image on our page.

<div class="filename">index.html</div>
```html
...
  <body>
    <h1>My Programming Goals</h1>
    <p>Every journey is easier if you <strong>know where you're going.</strong> <em>-unknown</em></p>

    <img src="https://tinyurl.com/lfkubwe" />

  </body>
...
```

Here we've added an element called an `<img>`. It's job is to show us an image. Note that there is no `</img>` present, instead the `/` is located at the end of the element itself. This is called a self-closing element.

 This element has additional information included, beyond what we've seen before. It has a **attribute** called `src`. This attribute defines the source of the image. In this case we're using a URL, to show an image from the internet. You can replace this URL with another image if you'd prefer, or a path from the HTML file to an image stored on your own computer.

<hr>

### An HTML list

Let's create a list of our goals below the image we're displaying. Add the following code below the `<img>` element.

<div class="filename">index.html</div>
```html
...
<h3>My Goals:</h3>
<p>
  I want to become a professional web developer. Here are the things I'll need to learn first.
</p>
<ul>
  <li>Learn HTML</li>
  <li>Learn CSS</li>
</ul>
...
```

* `<ul>` is an element that indicates we wish to display an un-ordered list. By default this means we'll display bullet points.
* `<li>` is a list item. When displayed within a list, they will be grouped together.

When we reload, we see our list neatly displayed.

<hr>

### Hyperlinks

Let's add one more element to our page. No website would be complete without links. They're important for linking pages together, and providing references to outside sites.

Let's add the following code to the *index.html* file.

<div class="filename">index.html</div>
```html
...
<h3>My favorite website</h3>
<h4><a href="http://www.google.com">Google</a></h4>
...
```

Here we've used another set of header elements and a new elements called an **anchor**. The anchor is defined with the `<a>` element. Notice that the anchor has an **attribute** just like an image. The `href` attribute is the hypertext reference. It declares where the anchor leads.

Now that we've finished with this section, our HTML looks pretty good. We have an image, a list, and a hyperlink. Let'm start making it look good with some CSS.
