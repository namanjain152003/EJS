EJS (Embedded JavaScript Templates)
EJS is a templating engine used with Node.js to generate HTML markup with plain JavaScript.

🔧 What Does EJS Do?
It lets you embed JavaScript logic (like loops, variables, if-else) directly inside HTML files. You can dynamically render content on your pages using EJS.


📄 Basic Syntax
Here’s a simple .ejs file:

<h1>Hello <%= name %></h1>
If you pass { name: 'Naman' } from the server, it renders:

html:
<h1>Hello Naman</h1>