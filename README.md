# 0x0F. Build a web app in JavaScript

In this project, you will finalize the previous project 0x0B. Implement a design with bootstrap and make some parts dynamic with Javascript (JQuery exactly).

You will reuse final files of 0x0B. Implement a design with bootstrap and update them.

You will use all HTML/CSS/Accessibility/Responsive design/Bootstrap/Javascript knowledges that you learned previously.

You won’t have a lot of instruction, you are free to implement it the way that you want - the objective is simple: Have fully functional web pages that look the same as the designer file.

**Note:** This webpage has been designed by Nicolas Philippot, UI/UX designer.

Here the final result:

### Web page: Homepage

**:desktop_computer: Desktop version**

<p align="center">
    <img src="img/Desktop/01_SMILESCHOOL_LANDING_desktop@2x.png" alt="desktop" width="25%" />
</p>

**:pager: Tablet version**

<p align="center">
    <img src="img/Tablet/01_SMILESCHOOL_LANDING_tablet@2x.png" alt="tablet" width="25%" />
</p>

**:iphone: Mobile version**

<p align="center">
    <img src="img/Mobile/01_SMILESCHOOL_LANDING_mobile@2x.png" alt="desktop" width="25%" />
</p>

### Web page: Pricing

**:desktop_computer: Desktop version**

<p align="center">
    <img src="img/Desktop/02_SMILESCHOOL_PRICING_desktop@2x.png" alt="desktop" width="25%" />
</p>

**:pager: Tablet version**

<p align="center">
    <img src="img/Tablet/02_SMILESCHOOL_PRICING_tablet@2x.png" alt="tablet" width="25%" />
</p>

**:iphone: Mobile version**

<p align="center">
    <img src="img/Mobile/02_SMILESCHOOL_PRICING_mobile@2x.png" alt="desktop" width="25%" />
</p>

### Web page: Courses

**:desktop_computer: Desktop version**

<p align="center">
    <img src="img/Desktop/03_SMILESCHOOL_COURSES_desktop@2x.png" alt="desktop" width="25%" />
</p>

**:pager: Tablet version**

<p align="center">
    <img src="img/Tablet/03_SMILESCHOOL_COURSES_tablet@2x.png" alt="tablet" width="25%" />
</p>

**:iphone: Mobile version**

<p align="center">
    <img src="img/Mobile/03_SMILESCHOOL_COURSES_mobile@2x.png" alt="desktop" width="25%" />
</p>

<br />

## Requirements

- You have to use Bootstrap
- Your `styles.css` must be as small as you can - **you must use as much as you can Bootstrap classes**
- You have to use JQuery
- Your `scripts.js` must contain all your Javascript part
- Your Javascript must be executed only when the document is loaded

## Imports

For this project, you will need: fonts from Google, JQuery, Bootstrap CSS/JS

        <link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap" rel="stylesheet">
        <link href="https://fonts.googleapis.com/css?family=Coiny&display=swap" rel="stylesheet">

        <script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>
        <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>

        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

        <link rel="stylesheet" href="styles.css">
        <script src="scripts.js"></script>

## Tasks
**0. Reuse and polish your Bootstrap integration:**

Copy files from `0x0B. Implement a design with bootstrap`:

- homepage.html -> [0-homepage.html](0-homepage.html)
- pricing.html -> [0-pricing.html](0-pricing.html)
- courses.html -> [0-courses.html](0-courses.html)
- [styles.css](styles.css) and any files/folders needed (images, fonts…)

And finalize the design if it’s not done yet - the final result should be the same as these screens:

- Homepage - fig file
- Pricing - fig file
- Courses - fig file

Important notes with Figma:

- if your computer doesn’t have missing fonts, you can find them here: source-sans-pro and Spin-Cycle-OT
- some values are in float - feel free to round them
- “Be pixel perfect” - yes! but mainly make sure colors, size and position are correct. #C271FF is not purple.

For this task, please write an amazing `README.md`

**Interactions note:**

- Web pages must switch to the tablet version when the screen width is 768px
- Web pages must switch to the mobile version when the screen width is 576px
- button hover/active: `opacity: 0.9`

<br />

[**1. Homepage - quotes:**](1-homepage.html)

From `0-homepage.html`, create `1-homepage.html`.

Replace static quotes by dynamic loading:

- URL: `https://smileschool-api.hbtn.info/quotes`
- No static quotes should be present in the quotes section
- During the Ajax request, a loader should be present
- Carousel should work like before

Example of my loader:

        HTML:
        <div class="loader"></div>

        CSS:
        .loader {
            border: 10px solid #f3f3f3;
            border-top: 10px solid #C271FF;
            border-radius: 50%;
            width: 80px;
            height: 80px;
            animation: spin 2s linear infinite;
            margin: auto;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

Final result:

![final-result-1](img/task1.gif)

