# College-Management-Portal
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>College Management Portal</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f6f9;
    }
    header {
      background: #2c3e50;
      color: #fff;
      padding: 15px;
      text-align: center;
    }
    nav {
      display: flex;
      background: #34495e;
    }
    nav a {
      flex: 1;
      padding: 14px;
      text-align: center;
      text-decoration: none;
      color: white;
      transition: background 0.3s;
    }
    nav a:hover {
      background: #1abc9c;
    }
    section {
      padding: 20px;
    }
    .card {
      background: white;
      padding: 20px;
      margin: 15px 0;
      border-radius: 8px;
      box-shadow: 0px 2px 5px rgba(0,0,0,0.1);
    }
    .btn {
      background: #1abc9c;
      border: none;
      color: white;
      padding: 10px 15px;
      cursor: pointer;
      border-radius: 5px;
    }
    .btn:hover {
      background: #16a085;
    }
    footer {
      text-align: center;
      padding: 15px;
      background: #2c3e50;
      color: white;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <header>
    <h1>College Management Portal</h1>
    <p>Welcome to XYZ College</p>
  </header>

  <nav>
    <a href="#" onclick="showSection('dashboard')">Dashboard</a>
    <a href="#" onclick="showSection('students')">Students</a>
    <a href="#" onclick="showSection('faculty')">Faculty</a>
    <a href="#" onclick="showSection('courses')">Courses</a>
    <a href="#" onclick="showSection('results')">Results</a>
  </nav>

  <section id="content">
    <!-- Default content -->
    <div id="dashboard" class="card">
      <h2>Dashboard</h2>
      <p>Select a module from the navigation bar to manage college records.</p>
    </div>

    <div id="students" class="card" style="display:none;">
      <h2>Student Module</h2>
      <p>View or manage student records here.</p>
      <button class="btn">Add New Student</button>
      <button class="btn">View Students</button>
    </div>

    <div id="faculty" class="card" style="display:none;">
      <h2>Faculty Module</h2>
      <p>Manage faculty details here.</p>
      <button class="btn">Add Faculty</button>
      <button class="btn">View Faculty</button>
    </div>

    <div id="courses" class="card" style="display:none;">
      <h2>Courses Module</h2>
      <p>Manage courses and subjects here.</p>
      <button class="btn">Add Course</button>
      <button class="btn">View Courses</button>
    </div>

    <div id="results" class="card" style="display:none;">
      <h2>Results Module</h2>
      <p>Upload and view student results here.</p>
      <button class="btn">Upload Result</button>
      <button class="btn">View Results</button>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 College Management Portal | Designed for BCA Project</p>
  </footer>

  <script>
    function showSection(sectionId) {
      let sections = document.querySelectorAll("#content > div");
      sections.forEach(sec => sec.style.display = "none");
      document.getElementById(sectionId).style.display = "block";
    }
  </script>

</body>
</html>
