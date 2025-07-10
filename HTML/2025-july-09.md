
# July 8, 2025  
## Work With Me Form — HTML & CSS Journal Entry

Today, I completed designing a "Work With Me" form using plain HTML and CSS. This component is part of my personal portfolio project and served as a practice in structuring and styling forms using front-end technologies only—no JavaScript or frameworks involved.

---

## Overview of the Form

The form is intended to gather essential details from individuals interested in working or collaborating with me. The input fields included are:

- Full Name (text field)
- Email Address (email field)
- Phone Number (telephone field)
- Gender (radio buttons: Male, Female, Prefer not to say)
- Work Experience (dropdown list)
- Availability (text input)
- Short Tagline (text input)
- About Yourself (textarea)
- LinkedIn Profile (URL input)
- GitHub Profile (URL input)
- Resume Link (URL input)
- Personal Website (URL input)
- Upload Profile Image (file input)

A submit button labeled **"Save Profile"** finalizes the form.

---

## HTML5 Input Types and Attributes

Each input element makes use of appropriate HTML5 types like:

- `text` for general inputs (e.g., name, tagline)
- `email` for email validation
- `tel` for phone entries
- `url` for social links and resume
- `file` for image uploads
- `radio` for gender options

Additional attributes were utilized to enhance the form:

- `required` to ensure certain fields must be filled before submission
- `placeholder` to give context inside inputs
- `accept="image/png, image/jpeg, image/gif"` to restrict the file input to images only
- `id` and `name` for every element to connect labels and enable data handling

---

## Layout and Structure Details

The structure is styled using internal CSS, embedded in the same HTML document.

Layout features:

- Flexbox was used to build a two-column responsive layout for wider screens
- On smaller viewports, it shifts into a single column via media queries
- Fields are grouped using container elements with classes like `.form-group`, `.row`, and `.col-half` for clarity

---

## Styling Strategy

I kept the styling minimal and clean, using internal CSS. Some design choices included:

- Uniform padding and margin to maintain spacing
- Rounded corners (`border-radius`) for form elements
- A subtle box-shadow on the form container for emphasis
- Default system fonts for readability
- A hover transition effect for the submit button to enhance interactivity

All of this was done without any third-party CSS libraries or frameworks.

---

## Why I Chose Gender Instead of Location

Typically, forms request the user's location, but in this case, I used gender identification. Radio buttons were selected because they allow users to pick only one option from a group. All buttons shared the same `name` to ensure mutual exclusivity.

The gender options included:

- Male  
- Female  
- Prefer not to say  

---

## Validation & Accessibility Practices

I made sure the form followed basic accessibility and validation guidelines:

- Labels are linked to their respective inputs using `for` and `id` attributes
- Input types like `email`, `url`, and `tel` assist in browser-based validation
- Placeholder values guide the user through form completion
- The `name` attribute is provided for every field, ensuring it's ready for backend use
- Fields are logically grouped and clearly labeled to improve user experience

---

## Key Learnings

Through this task, I practiced and understood how to:

- Organize and write well-structured HTML forms
- Choose appropriate input types for different data types
- Use form attributes like `required`, `id`, `name`, and `accept`
- Create a responsive form layout using Flexbox and media queries
- Style form elements without any external libraries or JS

Currently, this form is static with no backend integration. I may integrate it with a backend or third-party service in the future to handle submissions.
