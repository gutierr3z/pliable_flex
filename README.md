# Pliable CSS

It's a responsive layout structure (HTML/CSS) for a page that just needs a header at the top, content centered, and footer at the bottom.  Pliable is meant to be used when you want to keep things simple.  But can also work well hand in hand with heavy libraries like Bootstrap.  

## Getting Started

There are two steps in order to apply Pliable to a project.

### 1) Link to pliable.css

Your HTML file, index.html, needs to link to the /pliable/pliable.css.  

```
<link href="css/pliable/pliable.css" rel="stylesheet">
```
We assume that you are using a /css folder in your project.  If so, download the /pliable folder into your /css folder.  The file structure should now look like this:

```
your-project/css/pliable/
```
Now you are set to write your HTML.

### 2) Code HTML Tags

Pliable expects three top level tags as siblings; header, main, and footer.  We assume these will be the children of the body tag.

```
<body>
    <header></header>
    <main></main>
    <footer></footer>
</body>
```
Each of these tags needs to have two nested tags before any content.  We suggest these to be `<section>` tags but can be any block tags.  Pliable just expects two nested levels, does not look for specific types of tags.  

```
<body>
    <header>
        <section>
            <section>
                // content
            </section>
        </section>
    </header>
    <main>
        <section>
            <section>
                // content
            </section>
        </section>
    </main>
    <footer>
        <section>
            <section>
                // content
            </section>
        </section>
    </footer>
</body>
```