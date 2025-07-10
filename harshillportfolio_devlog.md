
# Development Log — `harshillportfolio`

This markdown file documents the process of building a simple one-page personal portfolio using only HTML and CSS. The project was created by a Computer Science undergraduate named Harshill, who had a basic understanding of web development and limited hands-on experience before this project.

## Overview of the Project

**Main Aim**  
To create a neat, responsive, and modern portfolio webpage that includes the following:
- Personal intro and greeting  
- About section  
- Educational and technical background  
- Space for projects  
- Contact section with social/media links  
- Display picture  

**Tech Stack Used**  
- HTML5  
- CSS3 (Flexbox, Grid, Media Queries)  
- External tools: Google Fonts, SVG icons  

The complete website was built and finalized on **July 7, 2025**.

## Project Folder Structure

```
/harshillportfolio/
├── index.html
├── style.css
├── assets/
│   └── profile.png
└── README.md
```

## Design & Planning Strategy

The layout was planned to be clean, understandable, and easy to navigate. All sections were arranged in a logical flow and written using semantic HTML for better readability and future edits.

### Core UI Elements

- **Navigation**: Stays fixed at the top. Uses anchor links to scroll to various sections. Active section highlighting is done via CSS.  
- **Hero Banner**: Contains a welcome message, my full name, a tagline ("Computer Science Student"), and two buttons — "View My Work" and "Contact Me".  
- **About Me**: Contains a short personal background, education journey, and present goals.  
- **Skills**: Organized into small cards showing programming knowledge, web development, and DSA.  
- **Projects**: Placeholder layout for upcoming work.  
- **Contact**: Clickable buttons for GitHub, LinkedIn, and email — each with hover effects.  

**Styling Approach**  
- **Theme**: Light background with contrasting dark and blue text  
- **Fonts**: Clean sans-serif with bold section headings  
- **Layout System**: Flexbox and Grid used for placing elements  
- **Responsiveness**: Designed mobile-first using media queries  

## Build Process & Fixes

### Initial Setup

- Wrote basic HTML boilerplate  
- Created `index.html` and `style.css`  
- Connected external font and stylesheet  
- Created and ordered main sections  

**Issue Faced**: Navbar overlapping page content  
**Fix Applied**: Added top padding to body same as navbar height.  

```css
body {
  padding-top: 60px;
}
```

### Hero Banner

This section was designed first. All text and buttons were centered using Flexbox.

**Issue Faced**: Buttons were not aligned well on smaller screens  
**Fix Applied**: Used media query to stack them vertically when screen width is reduced.

```css
@media (max-width: 600px) {
  .hero-buttons {
    flex-direction: column;
    gap: 12px;
  }
}
```

### About Section

This part had an image and some text. It discussed my academic experience and interest in tech.

**Problem**: Image wasn’t scaling well  
**Solution**: Used `max-width` and `object-fit` for responsiveness.

```css
img {
  max-width: 100%;
  object-fit: cover;
}
```

### Skills Display

Skills were grouped using a grid layout. Each group showed a different area like Programming, Web, and Data Structures.

**Design Note**: Created card-style sections with icon and short description.

### Project Showcase

Made basic cards for future projects. Each had a heading and some placeholder content.

**Problem**: Cards overflowed on small screens  
**Solution**: Set a max-width and used box-sizing to prevent layout breaking.

```css
.project-card {
  width: 100%;
  max-width: 300px;
  box-sizing: border-box;
}
```

### Contact Section

Added simple buttons with links to GitHub, LinkedIn, and email. Each had a hover effect for user feedback.

**Improvement Idea**: Add a contact form connected to backend later.

## Responsive Testing

Tested layout using browser dev tools for different screen sizes.

- Flexbox handled resizing and alignment well  
- Text remained readable at all screen widths  
- Buttons didn’t overflow and were easy to tap on touch devices  

Basic accessibility (like heading order and button tags) was followed, but full ARIA support is yet to be added.

## Issue Tracker & Solutions

| Problem                       | Cause                            | What I Did                                           |
|------------------------------|----------------------------------|------------------------------------------------------|
| Navbar hides top content     | No space added below navbar      | Used `padding-top` on body to fix it                 |
| Buttons wrap badly           | No responsive styling            | Applied media queries for better layout              |
| Image not scaling            | Missing constraints              | Used `max-width` and `object-fit`                    |
| Project cards break layout   | Fixed sizing without flexibility | Switched to % width and added `box-sizing`           |

## Personal Thoughts

This was my first complete project using raw HTML and CSS. Although I had watched videos and studied some theory, this was the first time applying it all in one go.

**Things That Went Well**  
- Finished main layout in a single day  
- Sections looked clean and well-organized  
- Mobile responsiveness worked smoothly  

**Things I Learned**  
- Planning section layout before writing code saves time  
- Layout bugs often come from missing `box-sizing` or overflow logic  
- Starting mobile-first makes things easier later  

## What’s Next?

- Add a downloadable resume  
- Expand projects with real links and descriptions  
- Add a working contact form (maybe with Formspree)  
- Clean up CSS or use SCSS for better structure  
- Deploy site to GitHub Pages or similar hosting  

**Final Build Completed On: July 7, 2025**
