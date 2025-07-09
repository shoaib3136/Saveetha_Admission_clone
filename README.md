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
  <title>Saveetha Engineering College Admission Enquiry</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <section class="main-container">
    <!-- Left Promotional Section -->
    <div class="left-section">
  <div class="branding">
    <img src="Screenshot 2025-07-09 185405-Photoroom.png" alt="Saveetha Engineering College Logo" class="college-logo">
    <div class="industry-text">
      <h1>INDUSTRY 5.0</h1>
      <p>Ready Curriculum Imparting</p>
      <p><strong>21st Century Skills</strong></p>
    </div>
  </div>
</div>

    <!-- Right Form Section -->
    <div class="right-section">
      <form class="admission-form">
        <h2>Admissions Open 2025</h2>

        <label for="name">Name</label>
        <input type="text" id="name" placeholder="Enter Name *" required>

        <label for="email">Email</label>
        <input type="email" id="email" placeholder="Enter Email Address *" required>

        <label for="phone">Mobile Number</label>
        <input type="tel" id="phone" placeholder="Enter Mobile Number *" required>

        <label for="password">Password</label>
        <input type="password" id="password" placeholder="Any Password of Your Choice *" required>

        <label for="state">State</label>
        <input type="text" id="state" placeholder="State *" required>

        <label for="city">City</label>
        <input type="text" id="city" placeholder="City *" required>

        <label for="course">Course</label>
        <input type="text" id="course" placeholder="Course *" required>

        <label for="specialization">Specialization</label>
        <input type="text" id="specialization" placeholder="Specialization *" required>
        <div class="checkbox-container">
          <input type="checkbox" id="consent" required>
          <label for="consent">I authorise Saveetha Engineering College to contact me via Email/SMS/WhatsApp/Call.</label>
        </div>

        <button type="submit">APPLY NOW</button>

        <p class="login-note">Already have an Account? <a href="#">Login</a> | <a href="#">Resend Verification Email</a></p>
      </form>
    </div>
  </section>
</body>
</html>

```

## CSS Code:
```css
/* styles.css */

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}

body {
  height: 100vh;
  overflow: hidden;
  background: url('college-image (1).jpg') no-repeat center center fixed;
  background-size: cover;
}

.main-container {
  display: flex;
  height: 100vh;
  width: 100vw;
  background-color: rgba(0, 0, 0, 0.6);
}

.left-section {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

.college-logo {
  max-width: 280px;
  width: 100%;
}

.right-section {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

.admission-form {
  width: 100%;
  max-width: 420px;
  background-color: #ffffff;
  border-radius: 10px;
  padding: 30px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
  overflow-y: auto;
  max-height: 90vh;
}

.admission-form h2 {
  color: #002f6c;
  margin-bottom: 20px;
  text-align: center;
}

.admission-form label {
  display: block;
  margin-bottom: 6px;
  font-weight: bold;
  font-size: 0.95rem;
}

.admission-form input[type="text"],
.admission-form input[type="email"],
.admission-form input[type="tel"],
.admission-form input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 14px;
}

.captcha-box {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 15px;
}

.captcha-box img {
  height: 40px;
}

.checkbox-container {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  font-size: 0.9rem;
  margin-bottom: 20px;
}

.checkbox-container input {
  margin-top: 5px;
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
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #e69500;
}

.login-note {
  font-size: 0.85rem;
  text-align: center;
  margin-top: 15px;
}

.login-note a {
  color: #0047ab;
  text-decoration: none;
}

.login-note a:hover {
  text-decoration: underline;
}

/* Responsive Design */
@media (max-width: 768px) {
  .main-container {
    flex-direction: column;
    overflow-y: auto;
  }

  .left-section,
  .right-section {
    flex: none;
    width: 100%;
    padding: 20px;
  }

  .admission-form {
    max-width: 90vw;
    max-height: 90vh;
  }

  .college-logo {
    max-width: 180px;
  }
}
.branding {
  text-align: center;
  color: white;
}

.college-logo {
  max-width: 380px; /* Increased from 280px */
  width: 100%;
  margin-bottom: 20px;
}

.industry-text h1 {
  font-size: 2.5rem;
  color: #ffde17;
  margin-bottom: 10px;
}

.industry-text p {
  font-size: 1.2rem;
  margin: 4px 0;
  color: #fff;
}


```

## Output:
![alt text](image-1.png)
## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
