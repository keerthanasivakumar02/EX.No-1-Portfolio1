## Ex01 Portfolio
## NAME: KEERTHANA S
## Date:04-03-2025
## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
# STEP 1
Create an HTML file (index.html)

# STEP 2
Create a CSS file (style.css)

# STEP 3
Include a navigation bar with links to different sections.

# STEP 4
Add structured sections for introduction, about, projects, and contact details.

# STEP 5
Define global styles for fonts, colors, and layout.

# STEP 6
Style the header, navigation bar, and sections.

# STEP 7
Use Flexbox or CSS Grid for layout design.

# STEP 8
Add hover effects and transitions for interactivity.

# STEP 9
Add Images and Media.

# STEP 10
Use optimized images for a professional look.

# STEP 11
Open the HTML file in a browser to check layout and functionality.

# STEP 12
Fix styling issues and refine content placement.

# STEP 13
Deploy the Portfolio.

# STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
# Main.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Keerthana Sivakumar | Portfolio</title>
  <link rel="stylesheet" href="style.css" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" />
</head>
<body>

  <!-- Navigation -->
  <nav>
    <div class="container nav-container">
      <a href="#" class="logo"><h2><span>Keerthana's Portfolio</span></h2></a>
      <ul>
        <li><a href="#About">About</a></li>
        <li><a href="#Services">Services</a></li>
        <li><a href="#Skills">Skills</a></li>
        <li><a href="#Contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- Header -->
  <header>
    <div class="header-container container">
      <div class="header-left">
        <h1>Hi, I'm <span>Keerthana Sivakumar</span></h1>
        <p>CSE Student</p>
        <p>
          I'm passionate about technology, coding, and problem-solving. I’m currently exploring
          web development, programming languages, and software engineering principles to grow as a developer.
        </p>
      </div>
      <div class="header-right">
        <img src="P2.jpg" alt="Keerthana's photo" />
      </div>
    </div>
  </header>

  <!-- About -->
  <section id="About">
    <h1><span>About Me</span></h1>
    <div class="container about-container">
      <p>
        I’m a Computer Science Engineering student eager to build and innovate through code.
        I enjoy learning new technologies, creating user-friendly websites, and working on challenging projects.
        My goal is to contribute meaningfully to real-world software development.
      </p>
    </div>
    <div class="about-content">
      <article class="about-article">
        <h5><span>Full Name</span></h5>
        <p>Keerthana Sivakumar</p>
      </article>
    </div>
  </section>

  <!-- Services -->
  <section id="Services">
    <h1><span>Services</span></h1>
    <div class="container services-container">
      <article class="services-article">
        <h2>Web Development</h2>
        <p>Creating responsive and interactive websites using HTML, CSS, and JavaScript.</p>
      </article>
      <article class="services-article">
        <h2>Problem Solving</h2>
        <p>Practicing data structures and algorithms to build strong coding skills.</p>
      </article>
    </div>
  </section>

  <!-- Skills -->
  <section id="Skills">
    <h1><span>Skills</span></h1>
    <div class="container skills-container">
      <article class="skill-article"><h4>HTML</h4></article>
      <article class="skill-article"><h4>CSS</h4></article>
      <article class="skill-article"><h4>JavaScript</h4></article>
      <article class="skill-article"><h4>Python</h4></article>
      <article class="skill-article"><h4>Problem Solving</h4></article>
    </div>
  </section>

  <!-- Contact -->
  <section id="Contact">
    <h1><span>Contact</span></h1>
    <div class="container contact-container">
      <form>
        <div class="form-top">
          <input type="text" placeholder="Name" required />
          <input type="email" placeholder="Email ID" required />
          <input type="text" placeholder="Message Subject" required />
        </div>
        <div class="form-bottom">
          <textarea name="message" placeholder="Your message" required></textarea>
          <button type="submit" class="btn btn-primary">Send Message</button>
        </div>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Keerthana Sivakumar
  </footer>

</body>
</html>





```
# style.css
```
/* Reset some default browser styling */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  }
  
  body {
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
  }
  
  .container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
  }
  
  /* Navigation */
  nav {
    background-color: #222;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 10;
  }
  
  .nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .logo h2 {
    color: #fff;
  }
  
  nav ul {
    list-style: none;
    display: flex;
    gap: 1.5rem;
  }
  
  nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
    transition: 0.3s;
  }
  
  nav ul li a:hover {
    color: #1abc9c;
  }
  
  /* Header Section */
  header {
    background-color: #1abc9c;
    color: #fff;
    padding: 4rem 0;
  }
  
  .header-container {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 2rem;
  }
  
  .header-left {
    flex: 1;
  }
  
  .header-right {
    flex: 1;
  }
  
  .header-right img {
    width: 100%;
    max-width: 300px;
    border-radius: 20px;
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  }
  
  /* Section Titles */
  section h1 {
    text-align: center;
    margin-top: 3rem;
    margin-bottom: 2rem;
    font-size: 2.5rem;
    color: #1abc9c;
  }
  
  /* About Section */
  .about-container,
  .about-content {
    margin-bottom: 2rem;
    text-align: center;
  }
  
  .about-article {
    margin: 1rem auto;
  }
  
  /* Services */
  .services-container {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: center;
  }
  
  .services-article {
    background: #fff;
    padding: 1.5rem;
    border-radius: 10px;
    width: 300px;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
  }
  
  /* Skills */
  .skills-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
  }
  
  .skill-article {
    background: #fff;
    padding: 1rem 2rem;
    border-radius: 25px;
    font-weight: bold;
    color: #1abc9c;
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
  }
  
  /* Contact */
  .contact-container form {
    background: #fff;
    padding: 2rem;
    max-width: 600px;
    margin: auto;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  }
  
  .form-top input,
  textarea {
    width: 100%;
    margin-bottom: 1rem;
    padding: 0.8rem;
    border-radius: 5px;
    border: 1px solid #ccc;
  }
  
  textarea {
    height: 100px;
  }
  
  .btn {
    background: #1abc9c;
    color: white;
    padding: 0.8rem 1.5rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
  }
  
  .btn:hover {
    background: #159c84;
  }
  
  /* Footer */
  footer {
    text-align: center;
    padding: 1rem 0;
    margin-top: 3rem;
    background: #222;
    color: #fff;
  }
  


```
## OUTPUT
![Screenshot 2025-04-25 185730](https://github.com/user-attachments/assets/34e081eb-2f1c-4076-ac05-b7b34dd41e14)

![Screenshot 2025-04-25 185820](https://github.com/user-attachments/assets/032d71c5-05a9-4a9a-9346-b612b35eae5b)

![Screenshot 2025-04-25 185852](https://github.com/user-attachments/assets/15a1c51b-5c37-440b-9d22-c1d87dd82433)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

No packages published
Footer
