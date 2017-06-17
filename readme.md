# > multivocal.org
### 🌊 🌊 🌊

Website for the Multivocal project.

**Uses:**
- KeystoneJS for blog CMS (also handles routing etc.)
- Handlebars for templating
- SCSS as the CSS preprocessor
- Gulp for compiling SCSS and minimizing JS (run ```gulp```, and I recommend the Livereload browser plugin)


## Guide 🤓

**How to set up locally**

- Clone project, then run ```npm install``` to install.
- Create a file called _.env_ in the root and write ```COOKIE_SECRET=whateverYouWant``` in it.
- Make sure Mongo is running (run ```mongod```)
- Run ```node keystone``` to start up, project lives on http://0.0.0.0:3000


**Writing a new blog post**

- Go to http://multivocal.org/keystone and log in with your user and password
- Create a new Post
- *State* should be set to Published (however, if you're not ready to publish, you can use the Draft option)
- *Content Brief* will show up in the list of blog posts
- *Content Extended* will show up on the blog post's page
- Make sure to clear all formatting in Content Brief and Content Extended (paste only plain text, and use the Clear Formatting button above the text field)
- For now, we don't use the *Categories*, so just ignore that :)
- Click *Save* and you're all good


**Change the static pages**

In order to change the static pages (Home, About, Contact) you need to edit the HTML.
The views can be found in _templates --> views_ and then the page you want to edit (e.g. _about.hbs_).
- Encapsulate text paragraphs in ```<p></p>```
- For headlines you can use ```<h2></h2>``` or ```<h3></h3>```
- For more info, refer to [this page](https://www.w3schools.com/html/html_basic.asp) 



✌️