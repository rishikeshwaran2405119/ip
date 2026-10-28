# Internet Programming Practical Repository (Experiments 1--10)

**Purpose:** Quick reference for the Internet Programming lab. Each
experiment has its own folder and the minimum files needed to run a
working demonstration.

> **Important:** This is a practical-ready reference implementation
> based on the experiment titles in the lab manual. Replace sample
> biodata with your own details. Keep image files in the same folder as
> the HTML that references them. For React/Angular/Node projects,
> install dependencies before running. Experiment 10 requires a running
> MySQL Server. Follow your college's rules about using online
> repositories during exams.

## Contents

1.  Static Web Page Using HTML5
2.  Auto Mechanic Shop Website Using HTML5
3.  WayFar Travel Website Using HTML & CSS
4.  Bootstrap Web Application 5(a). Television Shop Webpage with XML DTD
    5(b). Food Recipe Webpage with XML Schema 6(a). Marriage Validator
    Using JavaScript 6(b). Palindrome Checker Using JavaScript 6(c).
    Elective Course Registration Using JavaScript
5.  Angular Web Application
6.  Blog Articles Application Using ReactJS
7.  Event Registration Using Node.js
8.  CRUD Operations Using Node.js and MySQL

------------------------------------------------------------------------

## Experiment 1 --- Static Web Page Using HTML5

**Aim:** Display biodata using HTML5.

**Folder:** `Experiment-01`

Create `index.html`:

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>My Biodata</title>
</head>
<body>
  <header>
    <h1>MY BIODATA</h1>
    <h2>Your Name</h2>
    <address>Coimbatore, Tamil Nadu</address>
    <p>Email: yourname@example.com</p>
  </header>
  <article>
    <section>
      <h3>Objective</h3>
      <p>To learn, develop my skills, and contribute to an organization.</p>
    </section>
    <section>
      <h3>Education</h3>
      <table border="1">
        <tr><th>Course</th><th>Institution</th><th>Result</th></tr>
        <tr><td>SSLC</td><td>School Name</td><td>Percentage</td></tr>
        <tr><td>HSC</td><td>School Name</td><td>Percentage</td></tr>
        <tr><td>B.Tech IT</td><td>College Name</td><td>CGPA</td></tr>
      </table>
    </section>
    <section>
      <h3>Programming Skills</h3>
      <ul><li>Java</li><li>Python</li><li>HTML</li></ul>
    </section>
    <section>
      <h3>Projects</h3>
      <ol><li>Project One</li><li>Project Two</li></ol>
    </section>
  </article>
</body>
</html>
```

**Run:** Double-click `index.html` to open it in a browser. No
installation required.

**Keywords:** `<!DOCTYPE html>`, `<head>`, `<title>`, `<body>`,
`<header>`, `<article>`, `<section>`, `<table>`, `<ul>`, `<ol>`.

------------------------------------------------------------------------

## Experiment 2 --- Auto Mechanic Shop Website Using HTML5

**Aim:** Create Home, Services, Booking, and Contact pages.

**Folder:** `Experiment-02`

Create these four files in the same folder.

### `home.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Home | Auto Mechanic</title></head>
<body>
  <h1>Automob Mechanic</h1>
  <nav><a href="home.html">Home</a> | <a href="services.html">Services</a> |
       <a href="booking.html">Booking</a> | <a href="contact.html">Contact</a></nav>
  <h2>Your one-stop solution for car repair and service</h2>
  <p>We provide reliable vehicle maintenance and repair services.</p>
  <footer>Copyright © Auto Mechanic Shop</footer>
</body>
</html>
```

### `services.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Services</title></head>
<body>
  <h1>Our Services</h1>
  <nav><a href="home.html">Home</a> | <a href="services.html">Services</a> |
       <a href="booking.html">Booking</a> | <a href="contact.html">Contact</a></nav>
  <ul>
    <li>Preventive maintenance</li>
    <li>Engine repair</li>
    <li>Oil change</li>
    <li>Tyre service</li>
  </ul>
</body>
</html>
```

### `booking.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Book a Service</title></head>
<body>
  <h1>Service Booking</h1>
  <nav><a href="home.html">Home</a> | <a href="services.html">Services</a> |
       <a href="booking.html">Booking</a> | <a href="contact.html">Contact</a></nav>
  <form>
    <label>Full name: <input type="text" name="name" required></label><br><br>
    <label>Car model: <input type="text" name="model" required></label><br><br>
    <label>Car number: <input type="text" name="number" required></label><br><br>
    <label>Email: <input type="email" name="email" required></label><br><br>
    <label>Fuel:
      <select name="fuel"><option>Petrol</option><option>Diesel</option><option>Electric</option></select>
    </label><br><br>
    <label>Service:
      <select name="service"><option>Maintenance</option><option>Engine repair</option><option>Oil change</option></select>
    </label><br><br>
    <button type="submit">Book Service</button>
    <button type="reset">Reset</button>
  </form>
</body>
</html>
```

### `contact.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Contact</title></head>
<body>
  <h1>Contact Auto Mechanic</h1>
  <nav><a href="home.html">Home</a> | <a href="services.html">Services</a> |
       <a href="booking.html">Booking</a> | <a href="contact.html">Contact</a></nav>
  <p>Email: <a href="mailto:service@example.com">service@example.com</a></p>
  <p>Phone: 9876543210</p>
</body>
</html>
```

**Run:** Open `home.html` in a browser and use the navigation links. No
installation required.

**Keywords:** `<nav>`, `<a>`, `<form>`, `<input>`, `<select>`,
`<button>`, `<footer>`, `mailto:`.

------------------------------------------------------------------------

## Experiment 3 --- WayFar Travel Website Using HTML & CSS

**Aim:** Create a travel website with navigation and styled places.

**Folder:** `Experiment-03`

### `Home.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1">
  <title>WayFar Travel</title><link rel="stylesheet" href="style.css">
</head>
<body>
  <header><h1>WAYFAR TRAVEL</h1><p>Explore places. Make memories.</p></header>
  <nav><a href="Home.html">Home</a><a href="Places.html">Famous Places</a><a href="Booking.html">Ticket Booking</a></nav>
  <main class="card"><h2>Welcome to WayFar</h2><p>A comfort zone is a beautiful place, but nothing grows there.</p></main>
  <footer>Copyright © WayFar Travel</footer>
</body>
</html>
```

### `Places.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1">
<title>Famous Places</title><link rel="stylesheet" href="style.css"></head>
<body>
  <header><h1>Famous Places</h1></header>
  <nav><a href="Home.html">Home</a><a href="Places.html">Famous Places</a><a href="Booking.html">Ticket Booking</a></nav>
  <main class="grid">
    <div class="card">Coimbatore</div><div class="card">Chennai</div><div class="card">Erode</div>
    <div class="card">Salem</div><div class="card">Madurai</div><div class="card">Kumbakonam</div>
  </main>
  <footer>Copyright © WayFar Travel</footer>
</body>
</html>
```

### `Booking.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1">
<title>Ticket Booking</title><link rel="stylesheet" href="style.css"></head>
<body>
  <header><h1>Ticket Booking</h1></header>
  <nav><a href="Home.html">Home</a><a href="Places.html">Famous Places</a><a href="Booking.html">Ticket Booking</a></nav>
  <main class="card">
    <form><label>Name <input required></label><br><br>
    <label>Destination <input required></label><br><br>
    <label>Travel date <input type="date" required></label><br><br>
    <button>Submit</button></form>
  </main>
</body>
</html>
```

### `style.css`

``` css
body { margin: 0; font-family: Arial, sans-serif; background: #eaf6ff; }
header { text-align: center; padding: 25px; background: #9be3d2; color: #203a43; }
nav { display: flex; justify-content: center; gap: 20px; padding: 15px; background: #333; }
nav a { color: white; text-decoration: none; }
nav a:hover { color: yellow; }
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 15px; padding: 20px; }
.card { margin: 20px; padding: 20px; background: white; border: 1px solid #bbb; border-radius: 8px; }
footer { text-align: center; padding: 15px; }
```

**Run:** Open `Home.html`. Keep all HTML files and `style.css` in the
same folder.

**Keywords:** external CSS, `header`, `nav`, `display: flex`, CSS Grid,
`:hover`, `class`.

------------------------------------------------------------------------

## Experiment 4 --- Bootstrap Web Application

**Aim:** Build a responsive webpage using Bootstrap.

**Folder:** `Experiment-04`; create `index.html`.

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap Web Application</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-secondary">
    <div class="container">
      <a class="navbar-brand" href="#">My Website</a>
      <div class="navbar-nav">
        <a class="nav-link active" href="#">Home</a>
        <a class="nav-link" href="#about">About</a>
        <a class="nav-link" href="#contact">Contact</a>
      </div>
    </div>
  </nav>
  <main class="container my-4">
    <section id="about" class="p-4 bg-light rounded">
      <h1>Welcome</h1><p>This responsive website is built using Bootstrap 5.</p>
      <button class="btn btn-primary">Learn More</button>
    </section>
    <div class="row mt-4">
      <div class="col-md-4"><div class="card p-3 mb-3"><h3>Services</h3><p>Service details.</p></div></div>
      <div class="col-md-4"><div class="card p-3 mb-3"><h3>About Us</h3><p>About details.</p></div></div>
      <div class="col-md-4"><div class="card p-3 mb-3"><h3>Contact</h3><p id="contact">Contact details.</p></div></div>
    </div>
  </main>
</body>
</html>
```

**Run:** Open `index.html` in a browser. Internet is required to load
Bootstrap from the CDN.

**Keywords:** `container`, `navbar`, `row`, `col-md-4`, `card`, `btn`,
`bg-light`, responsive design.

------------------------------------------------------------------------

## Experiment 5(a) --- Television Shop Webpage with Data Verification Using XML DTD

**Aim:** Create TV data and describe its valid XML structure with an
internal DTD.

**Folder:** `Experiment-05a`

Create `television.xml`:

``` xml
<?xml version="1.0"?>
<?xml-stylesheet type="text/css" href="style.css"?>
<!DOCTYPE BEA [
  <!ELEMENT BEA (tv+)>
  <!ELEMENT tv (name,type,screen_size,resolution,price,viewing_angle,os)>
  <!ATTLIST tv brand CDATA #REQUIRED>
  <!ELEMENT name (#PCDATA)>
  <!ELEMENT type (#PCDATA)>
  <!ELEMENT screen_size (#PCDATA)>
  <!ELEMENT resolution (#PCDATA)>
  <!ELEMENT price (#PCDATA)>
  <!ELEMENT viewing_angle (#PCDATA)>
  <!ELEMENT os (#PCDATA)>
]>
<BEA>
  <tv brand="LG"><name>LG</name><type>LED</type><screen_size>32 inch</screen_size><resolution>1080p</resolution><price>40000</price><viewing_angle>20</viewing_angle><os>Android</os></tv>
  <tv brand="MI"><name>MI</name><type>OLED</type><screen_size>40 inch</screen_size><resolution>4K</resolution><price>50000</price><viewing_angle>30</viewing_angle><os>Google TV</os></tv>
  <tv brand="Sony"><name>Sony</name><type>LED</type><screen_size>42 inch</screen_size><resolution>4K</resolution><price>70000</price><viewing_angle>50</viewing_angle><os>Android</os></tv>
</BEA>
```

Create `style.css`:

``` css
BEA { display: block; margin: 10px; background: pink; font-family: Arial, sans-serif; }
tv { display: block; margin: 12px; padding: 12px; border: 1px solid #555; }
name { display: block; font-weight: bold; text-align: center; font-size: 20px; }
type, screen_size, resolution, price, viewing_angle, os { display: block; text-align: center; color: blue; }
```

**Run:** Open `television.xml` in a browser. Note: browsers may show XML
with CSS, but they do not all enforce DTD validation; use an XML
validator to validate the DTD.

**Keywords:** XML, root element, child element, `<!DOCTYPE>`,
`<!ELEMENT>`, `<!ATTLIST>`, `#PCDATA`, `#REQUIRED`.

------------------------------------------------------------------------

## Experiment 5(b) --- Food Recipe Webpage with Data Verification Using XML Schema

**Aim:** Create recipe data and validate its structure using an XML
Schema (XSD).

**Folder:** `Experiment-05b`

Create `food.xsd`:

``` xml
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:element name="food">
    <xs:complexType>
      <xs:sequence>
        <xs:element name="title" type="xs:string"/>
        <xs:element name="section" maxOccurs="unbounded">
          <xs:complexType>
            <xs:sequence>
              <xs:element name="name" type="xs:string"/>
              <xs:element name="i1" type="xs:string"/>
              <xs:element name="i2" type="xs:string"/>
              <xs:element name="i3" type="xs:string"/>
              <xs:element name="i4" type="xs:string"/>
              <xs:element name="recipe" type="xs:string"/>
            </xs:sequence>
          </xs:complexType>
        </xs:element>
      </xs:sequence>
    </xs:complexType>
  </xs:element>
</xs:schema>
```

Create `food.xml`:

``` xml
<?xml version="1.0" encoding="UTF-8"?>
<food xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:noNamespaceSchemaLocation="food.xsd">
  <title>Food Recipes</title>
  <section>
    <name>Noodles</name><i1>Water</i1><i2>Masala</i2><i3>Noodles</i3><i4>Salt</i4>
    <recipe>Boil water, add noodles and masala, and cook until soft.</recipe>
  </section>
  <section>
    <name>Kesari</name><i1>Rava</i1><i2>Sugar</i2><i3>Ghee</i3><i4>Saffron</i4>
    <recipe>Roast rava, add water and sugar, and cook with ghee.</recipe>
  </section>
</food>
```

Create `style.css`:

``` css
food, section, title, name, i1, i2, i3, i4, recipe { display: block; }
food { font-family: Arial, sans-serif; background: #fff7dc; padding: 15px; }
title { text-align: center; font-size: 28px; font-weight: bold; }
section { background: #e6f2c2; margin: 12px; padding: 12px; }
name { font-weight: bold; color: darkgreen; }
```

**Run:** Validate `food.xml` against `food.xsd` using an XML/XSD
validator. A browser may display XML, but may not perform XSD
validation.

**Keywords:** XSD, `xs:schema`, `xs:element`, `xs:complexType`,
`xs:sequence`, `type="xs:string"`, `maxOccurs`.

------------------------------------------------------------------------

## Experiment 6(a) --- Marriage Validator Using JavaScript

**Aim:** Check whether the bride and groom meet the age conditions in
the manual.

**Folder:** `Experiment-06a`; create `index.html`.

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"><title>Marriage Validator</title>
  <style>
    body { font-family: Arial; background: lavender; text-align: center; padding: 30px; }
    input, button { padding: 10px; margin: 8px; }
  </style>
</head>
<body>
  <h1>Marriage Validator</h1>
  <input type="number" id="bride" placeholder="Bride's age" min="1">
  <input type="number" id="groom" placeholder="Groom's age" min="1">
  <button onclick="check()">Validate</button>
  <p id="result"></p>
  <script>
    function check() {
      const bride = Number(document.getElementById("bride").value);
      const groom = Number(document.getElementById("groom").value);
      const result = document.getElementById("result");
      if (!bride || !groom) {
        result.textContent = "Please enter both ages.";
      } else if (bride >= 18 && groom >= 21) {
        result.textContent = "Marriage age conditions satisfied.";
      } else {
        result.textContent = "Marriage age conditions not satisfied.";
      }
    }
  </script>
</body>
</html>
```

**Run:** Open `index.html` in a browser. This reproduces the manual's
age thresholds for an academic exercise, not a complete legal
eligibility check.

**Keywords:** `function`, `document.getElementById()`, `.value`,
`Number()`, `if`, `else`, `onclick`, `textContent`.

------------------------------------------------------------------------

## Experiment 6(b) --- Palindrome Checker Using JavaScript

**Aim:** Check whether a word or phrase reads the same forward and
backward.

**Folder:** `Experiment-06b`; create `index.html`.

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"><title>Palindrome Checker</title>
</head>
<body>
  <h1>Palindrome Checker</h1>
  <input id="word" type="text" placeholder="Enter a word or phrase">
  <button onclick="checkPalindrome()">Check</button>
  <p id="result"></p>
  <script>
    function checkPalindrome() {
      const original = document.getElementById("word").value;
      const cleaned = original.toLowerCase().replace(/[^a-z0-9]/g, "");
      const reversed = cleaned.split("").reverse().join("");
      document.getElementById("result").textContent =
        cleaned && cleaned === reversed ? "Palindrome" : "Not a palindrome";
    }
  </script>
</body>
</html>
```

**Run:** Open `index.html`; try `madam`, `level`, or `hello`.

**Keywords:** `toLowerCase()`, `replace()`, `split()`, `reverse()`,
`join()`, comparison `===`, `onclick`.

------------------------------------------------------------------------

## Experiment 6(c) --- Elective Course Registration Using JavaScript

**Aim:** Validate login inputs and navigate to a course selection page.

**Folder:** `Experiment-06c`; create both files below. These are
demonstration credentials only---do not reuse them for real accounts.

### `index.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"><title>Elective Course Login</title>
</head>
<body>
  <h1>SREC Course Registration</h1>
  <form id="loginForm">
    <label>Username: <input type="text" id="user" required></label><br><br>
    <label>Password: <input type="password" id="pass" required></label><br><br>
    <button type="submit">Login</button>
    <button type="reset">Reset</button>
  </form>
  <p id="message"></p>
  <script>
    document.getElementById("loginForm").addEventListener("submit", function (event) {
      event.preventDefault();
      const username = document.getElementById("user").value.trim();
      const password = document.getElementById("pass").value;
      if (!username || !password) {
        document.getElementById("message").textContent = "Please fill both fields.";
      } else if (username === "2005034" && password === "srec@123") {
        alert("Login successful");
        window.location.href = "course-selection.html";
      } else {
        document.getElementById("message").textContent = "Invalid username or password.";
      }
    });
  </script>
</body>
</html>
```

### `course-selection.html`

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Course Selection</title></head>
<body>
  <h1>Elective Course Selection</h1>
  <form>
    <label>Select a course:
      <select required>
        <option value="">Choose one</option>
        <option>Artificial Intelligence</option>
        <option>Cloud Computing</option>
        <option>Cyber Security</option>
      </select>
    </label>
    <button type="submit">Register</button>
  </form>
</body>
</html>
```

**Run:** Open `index.html`. For this demonstration, use username
`2005034` and password `srec@123`. The credentials are client-side only
and are not secure for real authentication.

**Keywords:** `addEventListener`, `submit`, `preventDefault()`,
`.trim()`, `required`, `alert()`, `window.location.href`.

------------------------------------------------------------------------

## Experiment 7 --- Angular Web Application

**Aim:** Create a simple Angular application.

**Prerequisites:** Install Node.js LTS first, then open a new terminal.

``` bash
node -v
npm -v
npm install -g @angular/cli
ng new myNewApp
cd myNewApp
ng serve --open
```

If Angular asks configuration questions, choose the basic defaults. If
it asks whether to use SSR/SSG, choose No for this simple practical.

In current Angular CLI projects, the root files may be `src/app/app.ts`
and `src/app/app.html` (older manuals may show `app.component.ts` and
`app.component.html`). Edit the files actually generated by your
project.

### `src/app/app.ts` (current standalone naming)

``` typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  standalone: true,
  templateUrl: './app.html'
})
export class App {
  title = 'Welcome to Angular';

  changeTitle() {
    this.title = 'Angular Application';
  }
}
```

### `src/app/app.html`

``` html
<h1>{{ title }}</h1>
<button (click)="changeTitle()">Change Title</button>
```

**Run:** `ng serve --open`. The CLI displays the local URL, usually
`http://localhost:4200`.

**Keywords:** Angular, TypeScript, component, `@Component`,
interpolation `{{ }}`, event binding `(click)`, `ng new`, `ng serve`.

------------------------------------------------------------------------

## Experiment 8 --- Blog Articles Application Using ReactJS

**Aim:** Create a React blog app with Home, Blogs, Contact, and fallback
pages.

**Prerequisites:** Install Node.js. Create the project:

``` bash
npx create-react-app blogapp
cd blogapp
npm install react-router-dom
npm start
```

Create `src/App.js`:

``` jsx
import { BrowserRouter, Routes, Route, Link, Outlet } from "react-router-dom";

function Layout() {
  return (
    <>
      <nav>
        <Link to="/">Home</Link> | <Link to="/blogs">Blogs</Link> | <Link to="/contact">Contact</Link>
      </nav>
      <Outlet />
    </>
  );
}

function Home() { return <h1>Home Page</h1>; }
function Blogs() { return <h1>Blog Articles</h1>; }
function Contact() { return <h1>Contact Page</h1>; }
function NoPage() { return <h1>404 - Page Not Found</h1>; }

export default function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Layout />}>
          <Route index element={<Home />} />
          <Route path="blogs" element={<Blogs />} />
          <Route path="contact" element={<Contact />} />
          <Route path="*" element={<NoPage />} />
        </Route>
      </Routes>
    </BrowserRouter>
  );
}
```

**Run:** `npm start`. If the project is already cloned, run
`npm install` in the project folder first, then `npm start`.

**Keywords:** React, component, JSX, `BrowserRouter`, `Routes`, `Route`,
`Link`, `Outlet`, `npm start`.

------------------------------------------------------------------------

## Experiment 9 --- Event Registration Using Node.js

**Aim:** Receive event registration details using Node.js and Express.

**Prerequisites:** Install Node.js.

``` bash
mkdir Event
cd Event
npm init -y
npm install express
```

Create `index.html`:

``` html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Event Registration</title></head>
<body>
  <h1>Event Registration</h1>
  <form action="http://127.0.0.1:8000/example" method="get">
    <label>First name: <input name="firstname" required></label><br><br>
    <label>Last name: <input name="lastname" required></label><br><br>
    <label>About you: <input name="aboutyou"></label><br><br>
    <button type="submit">Register</button>
  </form>
</body>
</html>
```

Create `example.js`:

``` javascript
const express = require("express");
const app = express();

app.get("/example", (req, res) => {
  res.send(
    `<h1>Event Registration Successful</h1>
     <p>First Name: ${escapeHtml(req.query.firstname || "")}</p>
     <p>Last Name: ${escapeHtml(req.query.lastname || "")}</p>
     <p>About You: ${escapeHtml(req.query.aboutyou || "")}</p>`
  );
});

function escapeHtml(value) {
  return String(value).replace(/[&<>"']/g, char => ({
    "&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;", "'": "&#39;"
  })[char]);
}

app.listen(8000, () => console.log("Server running at http://127.0.0.1:8000"));
```

**Run:** 1. In the `Event` folder, run `node example.js`. 2. Open
`index.html` in the browser and submit the form. 3. Keep the terminal
open while testing.

**Keywords:** Node.js, Express, `require()`, `app.get()`, `req.query`,
`res.send()`, `app.listen()`, port 8000. GET query strings are for
demonstration; never send passwords this way.

------------------------------------------------------------------------

## Experiment 10 --- CRUD Operations Using Node.js and MySQL

**Aim:** Perform Create, Read, Update, and Delete operations on products
using Node.js and MySQL.

**Prerequisites:** MySQL Server must be installed and running. Keep your
database password private.

### Step 1 --- Create database and table

Open MySQL Workbench or the MySQL command-line client and run:

``` sql
CREATE DATABASE IF NOT EXISTS product;
USE product;

CREATE TABLE IF NOT EXISTS products (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  price DECIMAL(10,2) NOT NULL
);
```

### Step 2 --- Create Node project

``` bash
mkdir nodemysql
cd nodemysql
npm init -y
npm install express mysql
```

### Step 3 --- Create `server.js`

Replace `YOUR_MYSQL_PASSWORD` with your local MySQL root password. Do
not commit a real password to a public repository.

``` javascript
const express = require("express");
const mysql = require("mysql");
const app = express();

app.use(express.urlencoded({ extended: false }));
app.use(express.json());

const connection = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "YOUR_MYSQL_PASSWORD",
  database: "product"
});

connection.connect(err => {
  if (err) {
    console.error("MySQL connection failed:", err.message);
    process.exit(1);
  }
  console.log("Connected to MySQL");
});

app.get("/", (req, res) => {
  res.send(`
    <h1>Product CRUD</h1>
    <form method="post" action="/products">
      <input name="name" placeholder="Product name" required>
      <input name="price" type="number" step="0.01" min="0" placeholder="Price" required>
      <button type="submit">Add Product</button>
    </form>
    <p><a href="/products">View products</a></p>
  `);
});

// CREATE
app.post("/products", (req, res) => {
  const { name, price } = req.body;
  connection.query(
    "INSERT INTO products (name, price) VALUES (?, ?)",
    [name, price],
    err => {
      if (err) return res.status(500).send("Insert failed");
      res.redirect("/products");
    }
  );
});

// READ
app.get("/products", (req, res) => {
  connection.query("SELECT * FROM products", (err, rows) => {
    if (err) return res.status(500).send("Read failed");
    const list = rows.map(p =>
      `<li>${escapeHtml(p.name)} — ₹${p.price} 
       <form method="post" action="/products/${p.id}/delete" style="display:inline">
         <button type="submit">Delete</button>
       </form></li>`
    ).join("");
    res.send(`<h1>Products</h1><ul>${list}</ul><p><a href="/">Add another</a></p>`);
  });
});

// UPDATE: example endpoint for updating a product's price
app.post("/products/:id/update", (req, res) => {
  const id = Number(req.params.id);
  const price = Number(req.body.price);
  if (!Number.isInteger(id) || !Number.isFinite(price) || price < 0) {
    return res.status(400).send("Invalid product ID or price");
  }
  connection.query(
    "UPDATE products SET price = ? WHERE id = ?",
    [price, id],
    err => {
      if (err) return res.status(500).send("Update failed");
      res.redirect("/products");
    }
  );
});

// DELETE
app.post("/products/:id/delete", (req, res) => {
  const id = Number(req.params.id);
  if (!Number.isInteger(id)) return res.status(400).send("Invalid ID");
  connection.query("DELETE FROM products WHERE id = ?", [id], err => {
    if (err) return res.status(500).send("Delete failed");
    res.redirect("/products");
  });
});

function escapeHtml(value) {
  return String(value).replace(/[&<>"']/g, char => ({
    "&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;", "'": "&#39;"
  })[char]);
}

app.listen(8000, () => console.log("Open http://localhost:8000"));
```

**Run:** 1. Start MySQL Server. 2. Create the database/table with Step 1
SQL. 3. Set your password in `server.js`. 4. Run `node server.js`. 5.
Open `http://localhost:8000`.

**Note:** The sample demonstrates Create, Read, and Delete through the
browser. The Update endpoint is present but requires a POST request to
`/products/:id/update` with a `price` form field. This project uses the
`mysql` driver, consistent with the lab manual. Never push your actual
database password to GitHub.

**Keywords:** CRUD, MySQL, `mysql.createConnection()`,
`connection.connect()`, `connection.query()`, `INSERT`, `SELECT`,
`UPDATE`, `DELETE`, `WHERE`, primary key, `AUTO_INCREMENT`.

------------------------------------------------------------------------

## Fast GitHub setup and cloning

### Create a public repository

1.  Sign in to GitHub.
2.  Click **+** → **New repository**.
3.  Repository name: `internet-programming-practicals`.
4.  Choose **Public**.
5.  Select **Add a README file** and click **Create repository**.

### Add these folders and files

-   Fastest beginner method: on the repository page, click **Add file →
    Create new file**. Enter a path like `Experiment-01/index.html`,
    paste the matching code, then commit. Repeat for each file.
-   For many files, use Git locally: create the folder structure on your
    PC, save all files, then run the following commands from the main
    repository folder (replace the URL with your repository's actual
    URL):

``` bash
git init
git add .
git commit -m "Add Internet Programming experiments 1 to 10"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/internet-programming-practicals.git
git push -u origin main
```

If Git says the remote already exists, use
`git remote set-url origin https://github.com/YOUR-USERNAME/internet-programming-practicals.git`.

### Clone on the practical computer

Install Git if necessary, then:

``` bash
git clone https://github.com/YOUR-USERNAME/internet-programming-practicals.git
cd internet-programming-practicals
```

### Run quickly

-   HTML/CSS/Bootstrap/XML/JavaScript: open the relevant `.html` or
    `.xml` file in a browser. For XML Schema, use an XML validator to
    verify XSD.
-   Angular: open terminal in its project folder, run `npm install` if
    `node_modules` is missing, then `ng serve --open`.
-   React: run `npm install` if `node_modules` is missing, then
    `npm start`.
-   Node/Express: run `npm install` if needed, then `node example.js`.
-   Node/MySQL: ensure MySQL Server is installed/running and the
    database exists before `node server.js`.

## Final practical checklist

-   Test each experiment before the exam.
-   Check filenames and relative links carefully.
-   Keep image files in the same folder as their HTML pages.
-   Make sure Node.js, Git, and required database/software are installed
    on the exam computer.
-   `node_modules` is usually not committed; run `npm install` after
    cloning.
-   Public repositories are visible to everyone. Never commit passwords,
    personal data, or private college credentials.
-   Follow your college's rules about external code and internet use
    during practicals.
