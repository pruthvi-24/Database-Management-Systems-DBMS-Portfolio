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
  <p>I am an aspiring database professional passionate about designing efficient, secure, and reliable database systems.</p>
</section>

<section id="learning">
  <h2>Learning and Assignments</h2>

  <div class="assignment">
    <h3>4. Pharmaceutical Database Management</h3>
    <p><strong>Task:</strong> Design and manage a pharmaceutical database as per the given specifications.</p>
    <p><strong>Solution:</strong></p>
    <h4>1. ER Diagram</h4>
    <p>The ER diagram includes the following entities and relationships:</p>
    <ul>
      <li><strong>Entities:</strong>
        <ul>
          <li><strong>Pharmaceutical_Company</strong>: Company_Name (PK), Phone_No</li>
          <li><strong>Drug</strong>: Trade_Name (PK), Drug_Name, Formula, Company_Name (FK)</li>
          <li><strong>Pharmacy</strong>: Pharmacy_ID (PK), Name, Address, Phone_No</li>
          <li><strong>Patient</strong>: Patient_ID (PK), Name, Age, Address</li>
          <li><strong>Doctor</strong>: Doctor_ID (PK), Name, Specialty, Years_Experience</li>
          <li><strong>Prescription</strong>: Prescription_ID (PK), Doctor_ID (FK), Patient_ID (FK), Date, Quantity</li>
          <li><strong>Contract</strong>: Contract_ID (PK), Pharmacy_ID (FK), Company_Name (FK), Start_Date, End_Date, Terms, Supervisor</li>
        </ul>
      </li>
      <li><strong>Relationships:</strong>
        <ul>
          <li><strong>Sells</strong>: Between Pharmacy and Drug, with Price as an attribute.</li>
          <li><strong>Prescribes</strong>: Between Doctor and Patient, linked via Prescription.</li>
          <li><strong>Has_Contract</strong>: Between Pharmacy and Pharmaceutical_Company, linked via Contract.</li>
        </ul>
      </li>
    </ul>
    <h4>2. Relational Schema</h4>
    <p>The schema derived from the ER diagram includes:</p>
    <ul>
      <li>Pharmaceutical_Company: Company_Name (PK), Phone_No</li>
      <li>Drug: Trade_Name (PK), Drug_Name, Formula, Company_Name (FK)</li>
      <li>Pharmacy: Pharmacy_ID (PK), Name, Address, Phone_No</li>
      <li>Patient: Patient_ID (PK), Name, Age, Address</li>
      <li>Doctor: Doctor_ID (PK), Name, Specialty, Years_Experience</li>
      <li>Sells: Pharmacy_ID (PK, FK), Trade_Name (PK, FK), Price</li>
      <li>Prescribes: Prescription_ID (PK), Doctor_ID (FK), Patient_ID (FK), Date, Quantity</li>
      <li>Contract: Contract_ID (PK), Pharmacy_ID (FK), Company_Name (FK), Start_Date, End_Date, Terms, Supervisor</li>
    </ul>
    <h4>3. Sample Data</h4>
    <p>Populated tables with sample records:</p>
    <pre>
    Pharmaceutical_Company
    | Company_Name      | Phone_No    |
    |-------------------|-------------|
    | MedCorp           | 1234567890  |
    | HealthCare Ltd.   | 9876543210  |
    Drug
    | Trade_Name | Drug_Name   | Formula  | Company_Name   |
    |------------|-------------|----------|----------------|
    | Panadol    | Paracetamol | C8H9NO2  | MedCorp        |
    </pre>
    <h4>4. SQL Queries</h4>
    <p>Demonstrating concepts:</p>
    <ul>
      <li><strong>Multiple table join operations:</strong>
        <pre>
        SELECT Doctor.Name, Patient.Name, Drug.Trade_Name, Prescription.Quantity 
        FROM Prescription 
        JOIN Doctor ON Prescription.Doctor_ID = Doctor.Doctor_ID 
        JOIN Patient ON Prescription.Patient_ID = Patient.Patient_ID 
        JOIN Drug ON Prescription.Drug_ID = Drug.Trade_Name 
        WHERE Prescription.Quantity > 2;
        </pre>
      </li>
      <li><strong>Clauses & Functions:</strong>
        <pre>
        SELECT Pharmacy.Name, COUNT(Sells.Trade_Name) AS Drug_Count 
        FROM Pharmacy 
        JOIN Sells ON Pharmacy.Pharmacy_ID = Sells.Pharmacy_ID 
        GROUP BY Pharmacy.Name 
        HAVING COUNT(Sells.Trade_Name) > 3;
        </pre>
      </li>
      <li><strong>Subqueries:</strong>
        <pre>
        SELECT Name FROM Pharmacy 
        WHERE Pharmacy_ID = (SELECT Pharmacy_ID FROM Sells WHERE Trade_Name = 'Panadol');
        </pre>
      </li>
      <li><strong>Views:</strong>
        <pre>
        CREATE VIEW DrugPrices AS 
        SELECT Trade_Name, Pharmacy.Name, Price 
        FROM Sells 
        JOIN Pharmacy ON Sells.Pharmacy_ID = Pharmacy.Pharmacy_ID;
        </pre>
      </li>
    </ul>
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
