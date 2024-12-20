<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Database Management Systems - DBMS Portfolio</title>
  <style>
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
  <p>I am Pruthvi R, an aspiring database professional passionate about designing efficient, secure, and reliable database systems.</p>
</section>
<section id="learning">
  <h2>Learning and Assignments</h2>
  <div class="assignment">
    <h3>1. ER Model and Relational Algebra</h3>
    <p><strong>Assignment Name:</strong> "ER Model Design for a Library System"</p>
    <p><strong>Description:</strong> Designed entity types, relationships, and structural constraints to represent library database s
