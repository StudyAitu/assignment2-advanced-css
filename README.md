# Assignment #2 — Advanced CSS (Flexbox & Grid)

## Student Information

**Student:** Muratbek Ibrai
**Group:** SE-2529
**Assignment:** #2 — Advanced CSS (Flexbox & Grid)

---

## Project Overview

This project demonstrates the practical use of advanced CSS layout techniques, mainly **Flexbox** and **CSS Grid**.

The project contains four connected HTML pages. Each page demonstrates a different part of the assignment:

* Flexbox navigation bar
* Flexbox card row
* CSS Grid page layout with named areas
* CSS Grid image gallery
* Combination of Flexbox and Grid in a portfolio
* Responsive layouts for different screen sizes
* Hover effects and CSS transitions
* Reusable navigation between all pages

All pages use the same CSS file and the same navigation bar, which provides consistent design and easy navigation throughout the project.

The project was created using only **HTML5 and CSS3**, without external CSS frameworks or libraries.

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
```

---

## Technologies Used

* HTML5
* CSS3
* CSS Flexbox
* CSS Grid
* CSS Grid named areas
* CSS Media Queries
* CSS Transitions
* CSS Hover Effects
* Git
* GitHub
* GitHub Pages

**No external CSS frameworks or libraries were used.**

---

# Task 0 — Navigation Bar Using Flexbox

The navigation bar is implemented using **CSS Flexbox**.

The main navigation container uses:

```css
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
```

This allows the logo and navigation links to be placed horizontally and aligned properly.

The navigation links are also displayed using Flexbox:

```css
.nav-links {
    display: flex;
    gap: 24px;
}
```

The navigation contains links to all four pages:

* Flexbox
* Grid Layout
* Gallery
* Portfolio

The same navigation bar is reused on every page to provide consistent navigation throughout the project.

---

# Task 1 — Flexbox Card Row

The main Flexbox demonstration is located on `index.html`.

The cards are placed inside a Flexbox container:

```css
.card-row {
    display: flex;
    gap: 24px;
    flex-wrap: wrap;
}
```

Flexbox is used to:

* Arrange the cards horizontally
* Create equal spacing between cards
* Allow cards to wrap on smaller screens
* Create a responsive card layout

Each card contains:

* An image
* A title
* Descriptive text
* A button

The cards also include hover effects to improve visual interaction.

---

# Task 2 — CSS Grid Layout with Named Areas

The `layout.html` page demonstrates **CSS Grid with named grid areas**.

The main container uses:

```css
.grid-layout {
    display: grid;
    grid-template-columns: 240px 1fr;
    grid-template-rows: auto 1fr auto;
    grid-template-areas:
        "header header"
        "sidebar main"
        "footer footer";
}
```

The layout contains four main areas:

* Header
* Sidebar
* Main
* Footer

The corresponding elements are assigned to the named areas:

```css
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
```

This demonstrates how CSS Grid can be used to create a complete page structure using named areas.

---

# Task 3 — CSS Grid Image Gallery

The `gallery.html` page contains a gallery with **9 images**.

The gallery uses CSS Grid:

```css
.gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: 250px;
    gap: 18px;
}
```

The images are stored locally in the `images` folder:

* `g1.jpg`
* `g2.jpg`
* `g3.jpg`
* `g4.jpg`
* `g5.jpg`
* `g6.jpg`
* `g7.jpg`
* `g8.jpg`
* `g9.jpg`

Each image is placed inside a gallery item.

The gallery also includes a hover effect:

```css
.gallery-item:hover img {
    transform: scale(1.08);
}
```

A CSS transition is used to make the image enlargement smooth instead of changing instantly.

---

# Task 4 — Portfolio Using Flexbox and Grid

The `portfolio.html` page combines **CSS Grid and Flexbox** in the same interface.

CSS Grid is used for the main portfolio structure:

```css
.portfolio-layout {
    display: grid;
}
```

Flexbox is used inside the project cards to organize their content:

```css
.project-card {
    display: flex;
    flex-direction: column;
}
```

Each project contains:

* Project image
* Project title
* Project description
* Navigation button

The portfolio also contains an additional sidebar with information and skills.

This page demonstrates how **CSS Grid can control the overall page structure**, while **Flexbox can organize individual components inside the layout**.

---

# Responsive Design

The project includes responsive CSS using media queries.

For example:

```css
@media (max-width: 800px) {
    ...
}
```

and:

```css
@media (max-width: 520px) {
    ...
}
```

The responsive rules change the layout for smaller screen sizes.

Examples include:

* Navigation wrapping
* Cards becoming easier to fit on smaller screens
* Grid columns changing
* Sidebar and main content adapting to smaller widths
* Smaller spacing
* Adjusted typography
* More suitable layouts for mobile screens

This allows the pages to remain usable on different screen sizes.

---

# Hover Effects and Transitions

The project uses CSS transitions and hover effects for interactive elements.

Examples include:

* Navigation link hover effects
* Button hover effects
* Card hover effects
* Image scaling in the gallery
* Smooth transitions between normal and hover states

Example:

```css
.gallery-item:hover img {
    transform: scale(1.08);
}
```

The transition makes the image enlargement smooth and improves the visual interaction.

---

# File Description

### `index.html`

Contains the Flexbox navigation bar and the main Flexbox card row.

### `layout.html`

Demonstrates CSS Grid using named grid areas for the header, sidebar, main content and footer.

### `gallery.html`

Contains a 9-image CSS Grid gallery with hover effects and transitions.

### `portfolio.html`

Combines CSS Grid and Flexbox to create a responsive portfolio layout with projects and a sidebar.

### `css/style.css`

Contains the main CSS styles used by all HTML pages, including:

* Flexbox layouts
* CSS Grid layouts
* Grid named areas
* Responsive media queries
* Buttons
* Cards
* Gallery styles
* Hover effects
* CSS transitions
* General page styling

### `images/`

Contains all local images used by the project.

---

# Screenshots

The project contains four main pages:

1. Flexbox page
2. Grid Layout page
3. Gallery page
4. Portfolio page

The pages demonstrate the required Flexbox, Grid, responsive design and interactive effects.

---

# How to Run the Project

The project can be run locally using **IntelliJ IDEA** or any other web development environment.

### Option 1 — Open locally

Open the project folder and run:

```text
index.html
```

The other pages can be opened through the navigation bar.

### Option 2 — Open through GitHub Pages

The project is also published online using GitHub Pages.

All images and CSS files use relative paths, so the project does not depend on local absolute file paths.

---

# GitHub Pages

The project is published using GitHub Pages.

**Live Website:**

https://studyaitu.github.io/assignment2-advanced-css/

The published website contains all four pages and allows navigation between them.

---

# Result

The completed project demonstrates the practical use of:

* Flexbox
* CSS Grid
* CSS Grid named areas
* Responsive design
* CSS media queries
* CSS transitions
* Hover effects
* Reusable navigation
* Local image assets
* Combining Flexbox and Grid
* Multi-page website structure

The project contains all required HTML pages and uses a single shared stylesheet for consistent design.

---

# Conclusion

This assignment demonstrates how **Flexbox and CSS Grid** can be used to create structured, responsive and interactive web pages.

Flexbox was mainly used for one-dimensional layouts such as:

* Navigation bars
* Card rows
* Internal card content

CSS Grid was used for two-dimensional layouts such as:

* Main page structures
* Named grid areas
* Image galleries
* Portfolio layouts

The final project combines both techniques and demonstrates their practical use in a responsive multi-page website.

The project also demonstrates the use of CSS media queries, transitions and hover effects to improve responsiveness and user interaction.

