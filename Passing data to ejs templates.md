simple example of server to ejs


index.js:-

app.get("/", (req,res)=>{
    res.render("index.ejs", 
    { name: "naman" });
});


index.js:-

<body>
<h1>
HELLO <%= name %>
</h1>
</body>

if there is no data to send in ejs file but we declare the variable then it crashes our website 
so we should use locals keyword in ejs file so that it only takes data that is locally present in js file

