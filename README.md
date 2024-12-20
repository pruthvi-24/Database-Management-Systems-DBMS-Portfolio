<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Database Management Systems - DBMS Portfolio</title>
  <style>
    /* General Styling */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #000; /* Black Background */
      color: #FFD700; /* Yellow Text */
    }
    header {
      background-color: #1a1a1a;
      color: #FFD700;
      padding: 20px 10px;
      text-align: center;
    }
    .nav-links {
      list-style: none;
      padding: 0;
      margin: 20px 0 0;
      display: flex;
      justify-content: center;
      gap: 20px;
    }
    .nav-links a {
      text-decoration: none;
      color: #FFD700;
      font-weight: bold;
      padding: 5px 10px;
      transition: all 0.3s ease;
      background-color: transparent;
      border-radius: 4px;
    }
    .nav-links a:hover {
      color: #000;
      background-color: #FFD700; /* Yellow Background on Hover */
    }
    section {
      display: none; /* Hide sections by default */
      padding: 20px;
    }
    section.active {
      display: block; /* Show the active section */
    }
    footer {
      background-color: #1a1a1a;
      color: #FFD700;
      text-align: center;
      padding: 10px;
    }
    .github {
      text-align: center;
      margin-top: 30px;
    }
    .github a {
      color: #FFD700; /* Yellow color for GitHub links */
      text-decoration: none;
      font-weight: bold;
    }
    .github a:hover {
      color: #00acee; /* Blue on hover */
    }
    .assignment {
      background-color: #1a1a1a;
      padding: 15px;
      margin: 20px 0;
      border-radius: 8px;
      box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.2);
    }
    .assignment h3 {
      color: #FFD700; /* Yellow for assignment titles */
    }
    a {
      color: #FFD700; /* Default yellow color for links */
      text-decoration: none;
    }
    a:hover {
      color: #00acee; /* Blue on hover for consistency */
    }
  </style>
</head>
<body>

<header>
  <h1>Database Management Systems - DBMS Portfolio</h1>
  <p>Semester: 3 Semester | Department: Computer Science Engineering</p>
  <p>Mentor: Guruprasad Konnurmath | Course Code: 15ECSC208</p>
  <ul class="nav-links">
    <li><a href="#home" onclick="showSection('home')">Home</a></li>
    <li><a href="#about" onclick="showSection('about')">About Me</a></li>
    <li><a href="#learning" onclick="showSection('learning')">Learning and Assignments</a></li>
    <li><a href="#contact" onclick="showSection('contact')">Contact</a></li>
  </ul>
</header>

<section id="home" class="active">
  <h2>Home</h2>
  <p>Welcome to my DBMS portfolio. Here, I showcase my journey and accomplishments in learning database management systems.</p>
</section>

<section id="about">
  <h2>About Me</h2>
  <p>I am an aspiring database professional passionate about designing efficient, secure, and reliable database systems.</p>
</section>

<section id="learning">
  <h2>Learning and Assignments</h2>

  <div class="assignment">
    <h3>1. ER Model and Relational Algebra</h3>
    <p><strong>Assignment Name:</strong> "ER Model Design for a Library System"</p>
    <p><strong>Description:</strong> Designed entity types, relationships, and structural constraints to represent library database schema.</p>
    <p><strong>Challenges and Solutions:</strong> Efficiently handling many-to-many relationships using associative entities.</p>
    <p><strong>Reflection:</strong> Gained a solid understanding of ER modeling and relational algebra operations like SELECT and JOIN.</p>
  </div>

  <div class="assignment">
    <h3>2. SQL Database Creation</h3>
    <p><strong>Assignment Name:</strong> Created and queried a SQL database for pharmacy management.</p>
    <p><strong>Description:</strong> Used DDL and DML operations to create tables, insert data, and perform queries with aggregate functions.</p>
    <p><strong>Challenges and Solutions:</strong> Writing complex nested queries and debugging logical errors.</p>
    <p><strong>Reflection:</strong> Developed strong skills in SQL programming and query optimization.</p>
  </div>

  <div class="assignment">
    <h3>3. Normalization and Transaction Processing</h3>
    <p><strong>Assignment Name:</strong> Hospital Management System Normalization and Transactions.</p>
    <p><strong>Description:</strong> Normalized hospital database to 3NF and implemented ACID-compliant transaction processing.</p>
    <p><strong>Challenges and Solutions:</strong> Resolving partial and transitive dependencies for a large dataset.</p>
    <p><strong>Reflection:</strong> Learned how normalization improves database integrity and transaction management ensures consistency.</p>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>Email: <a href="mailto:01fe23bcs228@kletech.ac.in">01fe23bcs228@kletech.ac.in</a></p>
  <p>LinkedIn: <a href="https://linkedin.com/in/yourprofile" target="_blank">linkedin.com/in/yourprofile</a></p>
  <p>GitHub: <a href="https://github.com/yourprofile" target="_blank">github.com/yourprofile</a></p>
</section>

<div class="github">
  <h3>GitHub Repository</h3>
  <p>Check out the code for this portfolio on GitHub:</p>
  <a href="https://github.com/yourusername/Database-Management-Systems-DBMS-Portfolio" target="_blank">GitHub Repository Link</a>
</div>

<script>
  function showSection(sectionId) {
    const sections = document.querySelectorAll("section");
    sections.forEach((section) => {
      section.classList.remove("active");
    });
    document.getElementById(sectionId).classList.add("active");
  }
</script>

</body>
</html>
