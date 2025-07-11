# Saveetha_Admission_clone
## Date: 09-07-2025

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

   
    <div class="right-section">
      <form class="admission-form">
  <h2>Admissions Open 2025</h2>

  <div class="input-group">
    <i class="fa fa-user icon"></i>
    <input type="text" placeholder="Enter Name *" required>
  </div>

  <div class="input-group">
    <i class="fa fa-envelope icon"></i>
    <input type="email" placeholder="Enter Email Address *" required>
  </div>

  <div class="input-group">
    <i class="fa fa-phone icon"></i>
    <select class="country-code">
      <option value="+91">+91</option>
     
    </select>
    <input type="tel" placeholder="Enter Mobile Number *" required>
  </div>

  <div class="input-group">
    <i class="fa fa-lock icon"></i>
    <input type="password" placeholder="Any Password of Your Choice *" required>
  </div>

  <div class="flex-inputs">
    <div class="input-group">
      <i class="fa fa-map-marker icon"></i>
      <input type="text" placeholder="State *" required>
    </div>
    <div class="input-group">
      <i class="fa fa-map icon"></i>
      <input type="text" placeholder="City *" required>
    </div>
  </div>

  <div class="flex-inputs">
    <div class="input-group">
      <i class="fa fa-book icon"></i>
      <input type="text" placeholder="Course *" required>
    </div>
    <div class="input-group">
      <i class="fa fa-graduation-cap icon"></i>
      <input type="text" placeholder="Specialization *" required>
    </div>
  </div>

  

  <div class="checkbox-container">
    <input type="checkbox" id="consent" required>
    <label for="consent">I authorise Saveetha Engineering College & its representatives to contact me with updates and notifications via Email/SMS/WhatsApp/Call. This will override DND/NDNC *</label>
  </div>

  <button type="submit">APPLY NOW ▶</button>

  <p class="login-note">Already have an Account? <a href="#">Login</a> | <a href="#">Resend Verification Email</a></p>
</form>

    </div>
  </section>
</body>
</html>
```

## CSS Code:
```css

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
  background-color: rgba(67, 60, 60, 0.6);
  justify-content: center;
  align-items: center;
}


.left-section {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

.branding {
  text-align: center;
  color: white;
}

.college-logo {
  max-width: 380px;
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
  background-color: rgba(73, 67, 67, 0.6); 
  backdrop-filter: blur(3px); 
  border-radius: 10px;
  padding: 30px;
  color: white;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
  overflow: hidden;
  max-height: none;
}

.admission-form h2 {
  font-size: 1.6rem;
  font-weight: bold;
  color: #e1f905;
  background-color: #a79c9c;
  padding: 12px;
  border-radius: 8px;
  text-align: center;
  margin-bottom: 25px;
}


.input-group {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
  background-color: #fff;
  border-radius: 6px;
  padding: 10px;
}

.input-group .icon {
  color: #ff5e00;
  margin-right: 10px;
  font-size: 1.2rem;
}

.input-group input,
.input-group select {
  border: none;
  outline: none;
  width: 100%;
  font-size: 15px;
  background: none;
}

.country-code {
  width: 70px;
  margin-right: 10px;
}


.flex-inputs {
  display: flex;
  gap: 10px;
  margin-bottom: 15px;
}

.flex-inputs .input-group {
  flex: 1;
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
  font-weight: bold;
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
  color: #a8bad3;
  text-decoration: none;
}

.login-note a:hover {
  text-decoration: underline;
}


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
  }

  .college-logo {
    max-width: 180px;
  }
}
```

## Output:
![alt text](image-1.png)
## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
