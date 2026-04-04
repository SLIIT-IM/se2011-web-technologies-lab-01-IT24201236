[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ihYQzNJn)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23415985&assignment_repo_type=AssignmentRepo)
# SE2011---Web-Technologies---Lab-01

# Lab Sheet 01 – HTML Website Skeleton

**Module:** IT1100 – Internet and Web Technologies  
**Topic:** HTML Basics and Page Structure  
**Duration:** 2 Hours  
**Type:** Self-guided lab sheet  
**Output:** A complete multi-section website skeleton that will be improved in the next CSS and JavaScript lab sheets

This lab sheet is designed to match the HTML page structure, folder organization, and web-page development approach used in your lecture and earlier lab materials, where students first create the website structure in HTML, then style it with CSS, and later add interactivity with JavaScript. The earlier materials also use a project folder with separate `images`, `styles`, and `js` folders, and begin with building the page structure in `index.html`.

---

## 1. Learning outcomes

By the end of this lab, you should be able to:

- create the folder structure of a simple website
- create and save an HTML file correctly
- understand the basic structure of an HTML document
- use common HTML tags such as headings, paragraphs, images, links, lists, tables, forms, and semantic layout tags
- build the **skeleton** of a complete website using only HTML
- prepare the website properly for the next CSS and JavaScript labs

---

## 2. What you will build

In this lab, you will create the HTML structure for a simple website called:

**Campus Tech Store**

This is a simple student-friendly product website.  
In this lab, you will only create the **structure and content**.

In the next labs:

- **Lab 02 (CSS):** you will style this same website
- **Lab 03 (JavaScript):** you will add interactive features to this same website

So do not worry if the page looks plain at this stage.  
That is normal.  
This lab is about building the page correctly first.

---

## 3. Software needed

You can use any code editor such as:

- Visual Studio Code
- Notepad++
- Sublime Text
- even Windows Notepad

You also need a web browser such as:

- Google Chrome
- Microsoft Edge
- Firefox

---

## 4. Time plan for the 2-hour lab

### First hour

You will learn and build all the necessary HTML step by step.

### Last hour

You will complete a final task by extending the same webpage on your own using the instructions in this lab sheet.

---

## 5. Before you start: what is HTML?

HTML stands for **Hyper Text Markup Language**.  
It is the standard language used to create web pages.  
The browser reads HTML and displays the page content to the user. A basic HTML document contains `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>`. The lectures also introduce common HTML elements such as headings, paragraphs, images, and structural elements like header, footer, and navigation.

HTML is used to define the **structure** of the page.

For example:

- headings
- paragraphs
- images
- menus
- tables
- forms
- sections of a webpage

HTML is **not mainly for design**.  
Design will come later with CSS.

---

## 6. Create the project folder structure

Follow these steps very carefully.

### Step 1: Create the main folder

Create a folder named:

```text
IWT_Lab_01

```



### Step 2: Create subfolders inside it

Inside `IWT_Lab_01`, create these folders:

```text
IWT_Lab_01
│
├── src
│   ├── images
│   ├── styles
│   └── js

```

This kind of folder structure is consistent with the previous lab sheets, where students create a main folder and separate subfolders for images, styles, scripts, and the HTML file.

### Step 3: Create the HTML file

Inside the `src` folder, create a file named:

```text
index.html

```
So the location should be:

```text
IWT_Lab_01/src/index.html

```
## 7. Open the file in the editor

Open `index.html` in your code editor.

Type the following basic HTML structure:

```html
<!DOCTYPE html>  
<html>  
<head>  
    <title>Campus Tech Store</title>  
</head>  
<body>  
  
</body>  
</html>

```

## 8. Understand the basic HTML structure

Let us understand every line.

### `<!DOCTYPE html>`

This tells the browser that this is an HTML5 document.

**Why do we add it?**  
Because it helps the browser display the page in the correct modern standard.

### `<html> ... </html>`

This is the root element of the whole HTML page.

**Why do we add it?**  
Because all the HTML code must be inside this tag.

### `<head> ... </head>`

This section contains information **about** the page, not the visible page content.

**Why do we add it?**  
Because things like the page title and later CSS links are placed here.

### `<title>Campus Tech Store</title>`

This sets the page title shown on the browser tab.

**Why do we add it?**  
Because every web page should have a meaningful title.

### `<body> ... </body>`

This contains all the visible content shown in the browser.

**Why do we add it?**  
Because headings, images, menus, tables, and forms must appear inside the body.

These ideas directly match the lecture and lab content that explains the HTML document structure and the purpose of the `head` and `body` sections.

---

## 9. The website plan

We will build one single page with these parts:

1.  Header area  
2.  Navigation menu  
3.  Hero section  
4.  Product section  
5.  About section  
6.  Contact form  
7.  Footer  

This is good for learning because it includes many important HTML elements in one simple website.

---

## 10. Step-by-step website creation

---

### Step 10.1 – Add the page title and basic meta information

Replace your current code with this:

```html
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Campus Tech Store</title>  
</head>  
<body>  
  
</body>  
</html>

```

### Explanation

### `lang="en"`

This says the page language is English.

**Why do we add it?**  
Because it helps browsers, search engines, and accessibility tools understand the page language.

### `<meta charset="UTF-8">`

This allows the browser to correctly display many characters and symbols.

**Why do we add it?**  
Because without it, some characters may display incorrectly.

### `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

This helps the page behave better on mobile devices.

**Why do we add it?**  
Because modern web pages should work on different screen sizes.

---

## Step 10.2 – Add the website header

Now add this inside the `<body>` tag.

```html
<header>
    <img src="images/logo.png" alt="Campus Tech Store Logo" width="120">
    <h1>Campus Tech Store</h1>
    <p>Your student-friendly place for tech essentials</p>
</header>

```

### So now your body becomes:

```html
<body>  
    <header>  
        <img src="images/logo.png" alt="Campus Tech Store Logo" width="120">  
        <h1>Campus Tech Store</h1>  
        <p>Your student-friendly place for tech essentials</p>  
    </header>  
</body>


```

### Explanation

### `<header>`

This is a semantic HTML tag.

**Why do we add it?**  
Because it clearly tells the browser and developer that this part is the top section of the webpage.

### `<img>`

This is used to show an image.

**Why do we add it?**  
Because most websites have a logo or banner image.

### `src="images/logo.png"`

This tells the browser where the image file is located.

**Why do we add it?**  
Because the browser needs the file path to load the image.

### `alt="Campus Tech Store Logo"`

This gives alternative text.

**Why do we add it?**  
Because if the image does not load, or if a screen reader is used, this text explains the image.

### `width="120"`

This controls the image width.

**Why do we add it?**  
Because very large images may look too big on the page.

### `<h1>`

This is the main heading of the page.

**Why do we add it?**  
Because every page should have one main heading.

### `<p>`

This adds a paragraph.

**Why do we add it?**  
Because short descriptive text makes the page clearer.

### Important

You should place an image named `logo.png` inside the `images` folder.

Path:

```text
IWT_Lab_01/src/images/logo.png


```

### You can use any simple logo image.

---

## Step 10.3 – Add the navigation menu

Below the header, add this code:

```html
<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

```

### Explanation

### `<nav>`

This defines the navigation section.

**Why do we add it?**  
Because menus help users move around the page.

### `<ul>`

This creates an unordered list.

**Why do we add it?**  
Because menus are often built using list items.

### `<li>`

This means list item.

**Why do we add it?**  
Because each menu option is one item.

### `<a>`

This creates a hyperlink.

**Why do we add it?**  
Because clicking a menu item should move the user to the correct section.

### `href="#products"`

This links to an element with the matching `id`.

**Why do we add it?**  
Because it allows jumping to a section inside the same page.

---

## Step 10.4 – Add the home section

Now add a main content area and the first section.

### HTML:

```html
<main>
    <section id="home">
        <h2>Welcome to Campus Tech Store</h2>
        <p>
            We provide useful and affordable tech products for university students.  
            Explore laptops, headphones, smart watches, and accessories in one place.  
        </p>
        <img src="images/hero.jpg" alt="Students using technology" width="400">
    </section>
</main>


```

### Explanation

### `<main>`

This identifies the main content of the page.

**Why do we add it?**  
Because it separates the central content from header and footer.

### `<section>`

This groups related content together.

**Why do we add it?**  
Because each part of the webpage should be organized clearly.

### `id="home"`

This gives the section a unique name.

**Why do we add it?**  
Because the menu link `href="#home"` needs this `id` to work.

### `<h2>`

This is a second-level heading.

**Why do we add it?**  
Because the page already has one main heading `<h1>`, so section titles should usually start from `<h2>`.

---

## Step 10.5 – Add the product section

Inside `<main>`, after the home section, add this section.

### HTML:

```html
<section id="products">  
    <h2>Our Products</h2>  
    <p>Here are some popular items available for students.</p>  
  
    <table border="1">  
        <tr>  
            <th>Product Name</th>  
            <th>Description</th>  
            <th>Price</th>  
        </tr>  
        <tr>  
            <td>Laptop</td>  
            <td>Good for assignments, programming, and online lectures</td>  
            <td>Rs. 185000</td>  
        </tr>  
        <tr>  
            <td>Headphones</td>  
            <td>Useful for music, meetings, and video lessons</td>  
            <td>Rs. 8500</td>  
        </tr>  
        <tr>  
            <td>Smart Watch</td>  
            <td>Helps track time, fitness, and notifications</td>  
            <td>Rs. 12000</td>  
        </tr>  
    </table>  
</section>

```

### Explanation

### `<table>`

This creates a table.

**Why do we add it?**  
Because tables are useful for showing product data in rows and columns. Previous materials also use a product table in the web-page development lab.

### `border="1"`

This makes the table border visible.

**Why do we add it here?**  
Because we are still in the HTML lab. Later, in the CSS lab, you will style it properly.

### `<tr>`

This means table row.

### `<th>`

This means table heading cell.

**Why do we use `<th>` instead of `<td>` for the first row?**  
Because the first row contains labels such as Product Name, Description, and Price.

### `<td>`

This means table data cell.

**Why do we use it?**  
Because it holds the actual content.

---

## Step 10.6 – Add the about section

Below the products section, add:

### HTML:

```html
<section id="about">
    <h2>About Us</h2>
    <p>
        Campus Tech Store was created to help students find simple and affordable
        technology products for study and daily use.
    </p>
    <p>
        This website is built as a learning project for HTML, CSS, and JavaScript.
    </p>
</section>

```


### Explanation

This section uses simple paragraphs to describe the website.

**Why do we add this section?**  
Because most websites include some information about the business, service, or project.

---

## Step 10.7 – Add the contact section with a form

Below the about section, add:

### HTML:

```html
<section id="contact">
    <h2>Contact Us</h2>
    <form>
        <label for="fullname">Full Name:</label><br>
        <input type="text" id="fullname" name="fullname"><br><br>

        <label for="email">Email Address:</label><br>
        <input type="email" id="email" name="email"><br><br>

        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="5" cols="30"></textarea><br><br>

        <input type="submit" value="Send Message">
    </form>
</section>


```


### Explanation

Forms are introduced in your materials as an important part of web-based systems, and HTML forms are used to capture user data using input fields and related elements.

### `<form>`

This creates the form area.

**Why do we add it?**  
Because forms are used to collect user input.

### `<label>`

This gives a text label for an input field.

**Why do we add it?**  
Because users need to know what to enter.

### `for="fullname"`

This connects the label to the input with the same `id`.

**Why do we add it?**  
Because it improves clarity and accessibility.

### `<input type="text">`

This creates a one-line text box.

**Why do we add it?**  
Because the full name is short text.

### `<input type="email">`

This creates an email input field.

**Why do we use `email` type instead of `text`?**  
Because it is specifically meant for email addresses.

### `<textarea>`

This creates a larger text area.

**Why do we add it?**  
Because a message is usually longer than one line.

### `<input type="submit">`

This creates the submit button.

**Why do we add it?**  
Because forms usually need a button to send data.

At this stage, the form will not truly process data.  
That is okay.  
For now, we are learning page structure.

---

## Step 10.8 – Add the footer

After `</main>`, add:

### HTML:

```html
<footer>
    <hr>
    <p>&copy; 2026 Campus Tech Store. All rights reserved.</p>
    <p>Designed for IT1100 HTML Lab</p>
</footer>



```

### Explanation

This section uses simple paragraphs to describe the website.

**Why do we add this section?**  
Because most websites include some information about the business, service, or project.

---

## Step 10.7 – Add the contact section with a form

Below the about section, add:

### HTML:

```html
<section id="contact">
    <h2>Contact Us</h2>
    <form>
        <label for="fullname">Full Name:</label><br>
        <input type="text" id="fullname" name="fullname"><br><br>

        <label for="email">Email Address:</label><br>
        <input type="email" id="email" name="email"><br><br>

        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="5" cols="30"></textarea><br><br>

        <input type="submit" value="Send Message">
    </form>
</section>



```

### Explanation

Forms are introduced in your materials as an important part of web-based systems, and HTML forms are used to capture user data using input fields and related elements.

### `<form>`

This creates the form area.

**Why do we add it?**  
Because forms are used to collect user input.

### `<label>`

This gives a text label for an input field.

**Why do we add it?**  
Because users need to know what to enter.

### `for="fullname"`

This connects the label to the input with the same `id`.

**Why do we add it?**  
Because it improves clarity and accessibility.

### `<input type="text">`

This creates a one-line text box.

**Why do we add it?**  
Because the full name is short text.

### `<input type="email">`

This creates an email input field.

**Why do we use `email` type instead of `text`?**  
Because it is specifically meant for email addresses.

### `<textarea>`

This creates a larger text area.

**Why do we add it?**  
Because a message is usually longer than one line.

### `<input type="submit">`

This creates the submit button.

**Why do we add it?**  
Because forms usually need a button to send data.

At this stage, the form will not truly process data.  
That is okay.  
For now, we are learning page structure.

---

## Step 10.8 – Add the footer

After `</main>`, add:

### HTML:

```html
<footer>  
    <hr>  
    <p>&copy; 2026 Campus Tech Store. All rights reserved.</p>  
    <p>Designed for IT1100 HTML Lab</p>  
</footer>


```

### Explanation

### `<footer>`

This marks the bottom section of the webpage.

**Why do we add it?**  
Because websites usually end with ownership or copyright information.

### `<hr>`

This adds a horizontal line.

**Why do we add it?**  
Because it visually separates the footer from the main content.

### `&copy;`

This is the HTML entity for the copyright symbol.

**Why do we use it?**  
Because it correctly displays the copyright sign.

---

## 11. Full completed code

Now here is the full final code for `index.html`.

Copy it carefully if needed.

### HTML:

```html
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Campus Tech Store</title>  
</head>  
<body>  
  
    <header>  
        <img src="images/logo.png" alt="Campus Tech Store Logo" width="120">  
        <h1>Campus Tech Store</h1>  
        <p>Your student-friendly place for tech essentials</p>  
    </header>  
  
    <nav>  
        <ul>  
            <li><a href="#home">Home</a></li>  
            <li><a href="#products">Products</a></li>  
            <li><a href="#about">About</a></li>  
            <li><a href="#contact">Contact</a></li>  
        </ul>  
    </nav>  
  
    <main>  
        <section id="home">  
            <h2>Welcome to Campus Tech Store</h2>  
            <p>  
                We provide useful and affordable tech products for university students.  
                Explore laptops, headphones, smart watches, and accessories in one place.  
            </p>  
            <img src="images/hero.jpg" alt="Students using technology" width="400">  
        </section>  
  
        <section id="products">  
            <h2>Our Products</h2>  
            <p>Here are some popular items available for students.</p>  
  
            <table border="1">  
                <tr>  
                    <th>Product Name</th>  
                    <th>Description</th>  
                    <th>Price</th>  
                </tr>  
                <tr>  
                    <td>Laptop</td>  
                    <td>Good for assignments, programming, and online lectures</td>  
                    <td>Rs. 185000</td>  
                </tr>  
                <tr>  
                    <td>Headphones</td>  
                    <td>Useful for music, meetings, and video lessons</td>  
                    <td>Rs. 8500</td>  
                </tr>  
                <tr>  
                    <td>Smart Watch</td>  
                    <td>Helps track time, fitness, and notifications</td>  
                    <td>Rs. 12000</td>  
                </tr>  
            </table>  
        </section>  
  
        <section id="about">  
            <h2>About Us</h2>  
            <p>  
                Campus Tech Store was created to help students find simple and affordable  
                technology products for study and daily use.  
            </p>  
            <p>  
                This website is built as a learning project for HTML, CSS, and JavaScript.  
            </p>  
        </section>  
  
        <section id="contact">  
            <h2>Contact Us</h2>  
            <form>  
                <label for="fullname">Full Name:</label><br>  
                <input type="text" id="fullname" name="fullname"><br><br>  
  
                <label for="email">Email Address:</label><br>  
                <input type="email" id="email" name="email"><br><br>  
  
                <label for="message">Message:</label><br>  
                <textarea id="message" name="message" rows="5" cols="30"></textarea><br><br>  
  
                <input type="submit" value="Send Message">  
            </form>  
        </section>  
    </main>  
  
    <footer>  
        <hr>  
        <p>&copy; 2026 Campus Tech Store. All rights reserved.</p>  
        <p>Designed for IT1100 HTML Lab</p>  
    </footer>  
  
</body>  
</html>


```

## 12. What your project folder should look like now
--------------------------------------------------

```text
IWT_Lab_01  
│  
├── src  
│   ├── images  
│   │   ├── logo.png  
│   │   └── hero.jpg  
│   ├── styles  
│   ├── js  
│   └── index.html



```

## 13. How to run the website
---------------------------

1.  Save the file.
    
2.  Open the `src` folder.
    
3.  Double-click `index.html`.
    

Or:

1.  Right-click `index.html`
    
2.  Open with Chrome / Edge / Firefox
    

The browser will display your webpage.

---

## 14. Check your work
--------------------

Before moving to the final task, make sure:

- the page opens in the browser
- the title shows on the browser tab
- the logo image appears
- the menu links are visible
- the home, products, about, and contact sections are visible
- the table is visible
- the form fields are visible
- the footer is visible

---

## 15. Common mistakes and fixes
------------------------------

### Problem: Image is not showing

Check:

- is the image really inside the `images` folder?
- is the file name exactly correct?
- did you write `images/logo.png` correctly?

### Problem: Menu link does not move to section

Check:

- does the section have the matching `id`?
- for example, if the link is `href="#about"`, the section must be `id="about"`

### Problem: Page looks too plain

That is normal.  
This is only the HTML lab.  
In the next lab, you will add CSS styles.

### Problem: Code is not working

Check:

- are all opening tags closed properly?
- did you forget `>` or `</tag>` somewhere?
- did you save the file before opening it in the browser?

---

## 16. Final task for the second hour
-----------------------------------

Now complete this final task using the website you already created.

### Final Task: Extend the HTML page
--------------------------------

Add the following new features to your existing `index.html` file.

### Task A – Add a new section called “Student Offers”

Below the products section, add a new section with:

- a heading
- a short paragraph
- an ordered list with 3 offers

Example content:

- 10% discount for first-year students
- free delivery inside campus
- free laptop bag with selected items

### Task B – Add one more product row to the table

Add a fourth product to the table.

Example:

- Product Name: USB Flash Drive
- Description: Useful for storing and transferring files
- Price: Rs. 2500

### Task C – Add phone number field to the contact form

Add a new input field for phone number above the message box.

Use:

```html
<label for="phone">Phone Number:</label><br>
<input type="text" id="phone" name="phone"><br><br>


```

### Task D – Add one external link in the footer

Add a link to a useful technology website such as [W3Schools](https://www.w3schools.com/).

### HTML:

```html
<footer>
    <hr>
    <p>&copy; 2026 Campus Tech Store. All rights reserved.</p>
    <p>Designed for IT1100 HTML Lab</p>
    <p><a href="https://www.w3schools.com/" target="_blank">Visit W3Schools</a></p>
</footer>


```
### Why is this final task useful?

Because it helps you practice:

*   adding new sections
*   adding list elements
*   editing a table
*   editing a form
*   adding an external hyperlink

These are important HTML skills.

## 18. What will happen in the next lab
-------------------------------------

In the next lab sheet, you will use the **same website** and add CSS.

You will learn how to:

*   change colors
*   align content
*   style the navigation bar
*   improve the table
*   style the form
*   make the page look neat and attractive

This directly follows the progression in your earlier materials where structure comes first, then styling, then JavaScript behavior.

---

## 19. What to upload to GitHub
-----------------------------

Upload the whole project folder to your GitHub repository.

At minimum, your repository should contain:

```text
IWT_Lab_01/
└── src/
    ├── images/
    ├── styles/
    ├── js/
    └── index.html



```

## 20. Submission reminder
------------------------

Before submission, make sure:

*   your HTML file works
*   the images are included
*   the final task is completed
*   the file names are correct
*   the project is uploaded to GitHub properly


## 20. Submission reminder
------------------------

Before submission, make sure:

*   your HTML file works
*   the images are included
*   the final task is completed
*   the file names are correct
*   the project is uploaded to GitHub properly
