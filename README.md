# Assignment #2 — Advanced CSS (Flexbox & Grid)

## Student Information

- **Student:** Muratbek Ibrai
- **Group:** SE-2529
- **Assignment:** #2 — Advanced CSS (Flexbox & Grid)

---

## Project Overview

This project demonstrates the use of advanced CSS layout techniques, mainly **Flexbox** and **CSS Grid**.

The project contains four connected HTML pages. Each page demonstrates a different part of the assignment:

- Flexbox navigation bar
- Flexbox card row
- CSS Grid page layout with named areas
- CSS Grid image gallery
- Combination of Flexbox and Grid in a portfolio
- Responsive layouts for different screen sizes
- Hover effects and visual transitions

All pages use the same CSS file and the same navigation bar, which makes it possible to move between all parts of the project.

The project was created using only **HTML5 and CSS3** without external CSS frameworks.

---

## Project Structure

```text
assignment2-advanced-css/
│
├── index.html
├── layout.html
├── gallery.html
├── portfolio.html
├── README.md
│
├── css/
│   └── style.css
│
└── images/
    ├── logo.png
    ├── card1.jpg
    ├── card2.jpg
    ├── card3.jpg
    ├── proj1.jpg
    ├── proj2.jpg
    ├── g1.jpg
    ├── g2.jpg
    ├── g3.jpg
    ├── g4.jpg
    ├── g5.jpg
    ├── g6.jpg
    ├── g7.jpg
    ├── g8.jpg
    └── g9.jpg
Technologies Used
HTML5
CSS3
Flexbox
CSS Grid
CSS Grid named areas
CSS media queries
CSS tra nsitions
Git and GitHub
GitHub Pages
No external CSS frameworks or libraries were used.
Task 0 — Navigation Bar Using Flexbox
The navigation bar is implemented using CSS Flexbox.
The main navigation container uses:
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
This allows the logo and navigation links to be placed horizontally and aligned properly.
The navigation links are also displayed using Flexbox:
.nav-links {
    display: flex;
    gap: 24px;
}
The navigation contains links to all four pages:
Flexbox
Grid Layout
Gallery
Portfolio
The navigation is reused on all pages to provide consistent navigation throughout the project.
Task 1 — Flexbox Card Row
The main Flexbox demonstration is located on index.html.
The cards are placed inside a Flexbox container:
.card-row {
    display: flex;
    gap: 24px;
    flex-wrap: wrap;
}
Flexbox is used to:
arrange the cards horizontally
create equal spacing between cards
allow cards to wrap on smaller screens
create a responsive card layout
Each card contains:
an image
a title
descriptive text
a button
The cards also use hover effects to improve the visual interaction.
Task 2 — CSS Grid Layout with Named Areas
The layout.html page demonstrates CSS Grid with named grid areas.
The main container uses:
.grid-layout {
    display: grid;
    grid-template-columns: 240px 1fr;
    grid-template-rows: auto 1fr auto;
    grid-template-areas:
        "header header"
        "sidebar main"
        "footer footer";
}
The layout contains four main areas:
Header
Sidebar
Main
Footer
The corresponding elements are assigned to the named areas using:
.grid-header {
    grid-area: header;
}

.grid-sidebar {
    grid-area: sidebar;
}

.grid-main {
    grid-area: main;
}

.grid-layout > footer {
    grid-area: footer;
}
This demonstrates how CSS Grid can be used to create a complete page structure.
Task 3 — CSS Grid Image Gallery
The gallery.html page contains a gallery with 9 images.
The gallery uses CSS Grid:
.gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: 250px;
    gap: 18px;
}
The images are stored locally in the images folder:
g1.jpg
g2.jpg
g3.jpg
g4.jpg
g5.jpg
g6.jpg
g7.jpg
g8.jpg
g9.jpg
Each image is placed inside a gallery item.
The gallery also includes a hover effect:
.gallery-item:hover img {
    transform: scale(1.08);
}
A CSS transition is used to make the effect smooth.
Task 4 — Portfolio Using Flexbox and Grid
The portfolio.html page combines both CSS Grid and Flexbox.
CSS Grid is used for the main portfolio structure.
The project cards use Flexbox for their internal content layout.
Each project contains:
project image
project title
project description
navigation button
The portfolio also contains an additional sidebar with information and skills.
This page demonstrates how Flexbox and Grid can be combined in the same interface.
Responsive Design
The project includes responsive CSS using media queries.
For example:
@media (max-width: 800px) {
    ...
}
and:
@media (max-width: 520px) {
    ...
}
The responsive rules change the layout for smaller screens.
Examples include:
navigation wrapping
cards becoming easier to fit on smaller screens
Grid columns changing
sidebar and main content adapting to smaller widths
smaller spacing and typography
This allows the pages to remain usable on different screen sizes.
Hover Effects and Transitions
The project uses CSS transitions and hover effects for interactive elements.
Examples include:
navigation link hover effects
button hover effects
card hover effects
image scaling in the gallery
Example:
.gallery-item:hover img {
    transform: scale(1.08);
}
The transition makes the image enlargement smooth instead of changing instantly.
File Description
index.html
Contains the Flexbox navigation bar and Flexbox card row.
layout.html
Demonstrates CSS Grid layout using named grid areas for the header, sidebar, main content and footer.
gallery.html
Contains a 9-image CSS Grid gallery with hover effects.
portfolio.html
Combines CSS Grid and Flexbox to create a responsive portfolio layout.
css/style.css
Contains the main CSS styles used by all HTML pages, including:
Flexbox layouts
CSS Grid layouts
responsive media queries
buttons
cards
gallery styles
hover effects
transitions
images/
Contains all local images used in the project.
How to Run the Project
The project can be run locally using IntelliJ IDEA or any other web development environment.
Open the project folder and run:
index.html
The other pages can be opened through the navigation bar.
All images and CSS files use relative paths, so the project does not depend on local absolute file paths.
GitHub Pages
The project is published using GitHub Pages.
Live website:
https://studyaitu.github.io/assignment2-advanced-css/
The published website contains all four pages and allows navigation between them.
Result
The completed project demonstrates the practical use of:
Flexbox
CSS Grid
Grid named areas
Responsive design
CSS transitions
Hover effects
Reusable navigation
Local image assets
Combining Flexbox and Grid
The project contains all required HTML pages and uses a single shared stylesheet for consistent design.
Conclusion
This assignment helped demonstrate how Flexbox and CSS Grid can be used to create structured, responsive and interactive web pages.
Flexbox was mainly used for one-dimensional layouts such as navigation bars, card rows and internal card content.
CSS Grid was used for two-dimensional layouts such as the main page structure, gallery and portfolio.
The final project combines both techniques and demonstrates their practical use in a responsive multi-page website.
