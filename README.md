</style>
</head>
<body>

<header>
  <h1>Database Management Systems - DBMS Portfolio</h1>
  <p>Semester: 3 Semester | Department: Computer Science Engineering</p>
  <p>Contact: <a href="mailto:01fe23bcs228@kletech.ac.in" style="color: #FFD700;">01fe23bcs228@kletech.ac.in</a></p>
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

<footer>
  <p>&copy; 2024 All Rights Reserved.</p>
</footer>

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
