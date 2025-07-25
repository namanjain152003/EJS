ejs can be used to remove repetive part of code..

 In EJS, partials are reusable chunks of HTML (or EJS) code — like components — that you can include in multiple pages. They're commonly used for headers, footers, navbars, etc.


  Why use partials?
To avoid repeating the same code in every file.

views/
├── partials/
│   ├── header.ejs
│   └── footer.ejs
├── home.ejs
└── about.ejs



partials/header.ejs:-

<!DOCTYPE html>
<html>
<head>
  <title>My Site</title>
</head>
<body>
  <h1>Welcome!</h1>
  <nav>
    <a href="/">Home</a> | <a href="/about">About</a>
  </nav>


 partials/footer.ejs:-

   <footer>
    <p>© 2025 My Website</p>
  </footer>
</body>
</html>


home.ejs:-

<%- include("partials/header") %>

<h2>This is the homepage</h2>

<%- include("partials/footer") %>



about.ejs:-

<%- include("partials/header") %>

<h2>This is the about page</h2>

<%- include("partials/footer") %>


