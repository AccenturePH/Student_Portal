<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Portal</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* Custom styles for the E-Library section */
    .e-library {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
      padding: 20px;
      background-color: #f5f5f5;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    
    .e-library-box {
      background-color: #fff;
      border: 1px solid #ddd;
      padding: 20px;
      border-radius: 8px;
      text-align: center;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .e-library-box h3 {
      font-size: 18px;
      margin-bottom: 10px;
    }

    .e-library-box a {
      text-decoration: none;
      color: #4a90e2;
      font-weight: bold;
    }

    .e-library-box a:hover {
      text-decoration: underline;
    }

    .e-library-header {
      text-align: center;
      margin-bottom: 30px;
    }

    .e-library-header h2 {
      font-size: 24px;
      font-weight: bold;
      color: #333;
    }

    .e-library-section {
      display: none;
    }

  </style>
</head>
<body>
  <header class="portal-header">
    <div class="student-info">
      <img src="profile-picture.jpg" alt="Student Photo" class="student-photo">
      <div class="info">
        <h1>Juan Dela Cruz</h1>
        <p><b>First Semester AY 2024-2025</b></p>
        <p>BS Business Administration - First Year</p>
        <p>Status: <span class="status">Enrolled</span></p>
      </div>
    </div>
  </header>

  <nav class="navigation">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">News</a></li>
      <li><a href="#">Advisories</a></li>
      <li><a href="#">Schedules</a></li>
      <li><a href="#">Downloads</a></li>
      <li><a href="#" onclick="showELibrary()">E-Library</a></li>
    </ul>
  </nav>

  <main>
    <section class="services">
      <h2>Enrollment - First Semester AY 2024-2025</h2>
      <div class="service-grid">
        <a href="#">Certificate of Registration</a>
        <a href="#">Grades</a>
        <a href="#">Scholarships</a>
        <a href="#">Assessment of Fees</a>
        <a href="#">Payments</a>
        <a href="#">Student ID</a>
        <a href="#">Subjects</a>
        <a href="#">Curriculum</a>
      </div>
    </section>

    <section class="others">
      <h2>Other Links</h2>
      <div class="service-grid">
        <a href="#">Online Public Access Catalog</a>
        <a href="#">My QR Code</a>
        <a href="#">Student Information Sheet</a>
        <a href="#">Vaccination Status</a>
      </div>
    </section>

    <!-- E-Library Section -->
    <section class="e-library-section" id="elibrary">
      <div class="e-library-header">
        <h2>E-Library</h2>
        <p>Explore the latest books, journals, and e-books in Business Administration</p>
      </div>

      <div class="e-library">
        <div class="e-library-box">
          <h3>Administration Books</h3>
          <a href="#">View Books</a>
        </div>

        <div class="e-library-box">
          <h3>Management Journals</h3>
          <a href="#">View Journals</a>
        </div>

        <div class="e-library-box">
          <h3>Business E-books</h3>
          <a href="#">View E-books</a>
        </div>

        <div class="e-library-box">
          <h3>Finance & Marketing Resources</h3>
          <a href="#">View Resources</a>
        </div>

        <div class="e-library-box">
          <h3>Entrepreneurship Books</h3>
          <a href="#">View Books</a>
        </div>

        <div class="e-library-box">
          <h3>Accounting Journals</h3>
          <a href="#">View Journals</a>
        </div>
      </div>
      <button onclick="hideELibrary()">Back to Portal</button>
    </section>

  </main>

  <footer class="footer">
    <p>© 2024 Accenture Services. All Rights Reserved.</p>
  </footer>

  <script>
    // Show E-Library Section
    function showELibrary() {
      document.querySelector('.services').style.display = 'none';  // Hide the portal content
      document.querySelector('.others').style.display = 'none';  // Hide the portal content
      document.getElementById('elibrary').style.display = 'block';  // Show E-Library content
    }

    // Hide E-Library Section and return to portal
    function hideELibrary() {
      document.querySelector('.services').style.display = 'block';  // Show portal content
      document.querySelector('.others').style.display = 'block';  // Show portal content
      document.getElementById('elibrary').style.display = 'none';  // Hide E-Library content
    }
  </script>
</body>
</html>
# Student_Portal
