# Saveetha_Admission_clone
## Date:

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saveetha Engineering College Admissions 2025</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="overlay">
        <header>
            <img src="saveetha logo.png" alt="Saveetha Engineering College Logo" class="logo">
        </header>

         <div class="form-container">
      <h2>Admissions Open 2025</h2>
      <form>
        <input type="text" placeholder="Enter Name *" required>
        <input type="email" placeholder="Enter Email Address *" required>
        <input type="tel" placeholder="Enter Mobile Number *" required>
        <input type="password" placeholder="Any Password of Your Choice *" required>
        <input type="text" placeholder="State *" required>
        <input type="text" placeholder="City *" required>
        <input type="text" placeholder="Course *" required>
        <input type="text" placeholder="Specialization *" required>
        <label class="checkbox">
          <input type="checkbox" required>
          I authorise Saveetha Engineering College to contact me via Email/SMS/WhatsApp/Call.
        </label>

        <button type="submit">APPLY NOW</button>
      </form>
      <p class="login-note">Already have an Account? <a href="#">Login</a> | <a href="#">Resend Verification Email</a></p>
    </div>
    </div>
</body>
</html>

```

## CSS Code:
```css
body {
    margin: 0;
    padding: 0;
    background: url('college-image (1).jpg') no-repeat center center fixed;
    background-size: cover;
    font-family: Arial, sans-serif;
}

.overlay {
    background-color: rgba(0, 0, 0, 0.6);
    min-height: 100vh;
    padding: 20px;
    box-sizing: border-box;
}

.logo {
    width: 300px;
    display: block;
    margin: 0 auto 20px;
}

.form-container {
    max-width: 400px;
    background: white;
    padding: 30px;
    margin: auto;
    border-radius: 10px;
    box-shadow: 0 0 20px rgba(255, 255, 255, 0.2);
    text-align: center;
}

.form-container h2 {
    margin-bottom: 20px;
    color: #002f6c;
}

form input[type="text"],
form input[type="email"],
form input[type="tel"],
form input[type="password"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 12px;
    border: 1px solid #ccc;
    border-radius: 5px;
}
.form-container {
  flex: 1;
  max-width: 450px;
  background-color: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 0 25px rgba(255, 255, 255, 0.2);
  text-align: center;
}

.dropdowns input {
    width: 48%;
    margin: 1%;
}

.captcha {
    display: flex;
    align-items: center;
    gap: 10px;
    margin: 15px 0;
}



.checkbox {
    font-size: 0.9rem;
    display: block;
    text-align: left;
    margin: 10px 0;
}

button {
    width: 100%;
    padding: 12px;
    background-color: orange;
    color: white;
    border: none;
    border-radius: 6px;
    font-size: 1rem;
    cursor: pointer;
}

.login-note {
    font-size: 0.85rem;
    color: #333;
    margin-top: 10px;
}

```

## Output:
![alt text](image.png)
## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
