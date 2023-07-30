
<html>
<head>
  <title>My Resume</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #180202;
      padding: 20px;
    }

    h1 {
      text-align: center;
      text-decoration: underline;
      color: #ebdede;
      margin-bottom: 30px;
    }
    h2{
      color:#ffffff;
    }

    .section {
      margin-bottom: 30px;
      padding: 20px;
      background-color: #ffeecc;
      border-radius: 5px;
  
    }
    
    
    .profile-image {
      display: block;
      margin: 0 auto;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      box-shadow: 0 2px 4px rgba(216, 210, 210, 0.1);
    }

    .section h2 {
      margin-bottom: 10px;
      color: #150404;
    }

    .section p {
      margin: 0;
      color: #150606;
    }
    


    .section ul {
      margin: 0;
      padding-left: 20px;
      color: #1e0b0b;
    }
    
    .section ol {
      margin: 0;
      padding-left: 20px;
      color: #1e0b0b;
    }

    .contact-table {
      width: 100%;
      max-width: 500px;
      margin: 1 ;
      border: #150404;
    }

    .contact-table th {
      text-align: left;
      padding-right: 10px;
     
    }

    a {
      color: white;
    }

   
    a[href^="https://"] {
      color: rgb(225, 225, 230);
      float: left;
    }

    @media screen and (max-width: 600px) {
      .section {
        padding: 10px;
      }

      .profile-image {
        width: 120px;
        height: 120px;
      }

      @media screen and (min-width: 601px) {
      .section {
        padding: 12px;
      }

      .profile-image {
        width: 200px;
        height: 200px;
      }  

    }
  </style>
</head>
<body>
  <h1>Rehaan's Resume</h1>

  <div class="section">
    <img class="profile-image" src="C:\Users\test\Desktop\CSE103 lab2\html\Resume\my Image 2023-05-27 at 11.47.15.jpg" alt="My Image">
    <h2>Contact Information:</h2>
    <p><strong>Name:</strong>  SHAIK REHAAN ASHRAF</p>
    <p><strong>Email:</strong>  <a href="mailto:rehaanashraf2005@gmail.com" style="text-decoration: none; color: black;">rehaanashraf2005@gmail.com</a></p>
    <p><strong>Phone:</strong><a href="tel:8008556781" style="color: #150404;text-decoration: none; "> 8008556781</a></p>
    <p><strong>Address:</strong> MAGUNTA LAYOUT, VILLA N0-7, NELLORE</p>
  </div>

  <div class="section objective">
    <h2>Objective:</h2>
    <p>Highly motivated and results-oriented professional seeking a challenging position in computer programming to utilize my skills and contribute to the success of the organization. Committed to continuous learning and growth, I aim to leverage my specific expertise to drive specific outcomes while delivering exceptional value to clients, customers, and stakeholders.</p>
  </div>

  <div class="section">
    <h2>Education:</h2>
    <table >
      <tr>
        <th>School:</th>
        <td>ICSE in Redbridge International Academy.</td>
      </tr>
      <tr>
        <th>Degree:</th>
        <td>Bachelor of technology in Computer Science</td>
      </tr>
      <tr>
        <th>University:</th>
        <td>AMRITA VISHWA VIDYAPEETAM</td>
      </tr>
      <tr>
        <th>Year:</th>
        <td>2023</td>
      </tr>
      
    </table>
  </div>

  <div class="section">
    <h2>Skills:</h2>
    <ol>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>Python</li>
      <li>C</li>
    </ol>
  </div>

  <div class="section">
    <h2>Hobbies:</h2>
    <ul>
      <li>Gaming</li>
      <li>Painting</li>
      <li>Origami</li>
      <li>Listening to Music</li>
    </ul>
  </div>
  <h2>For More Info :</h2>
  <a href="https://www.linkedin.com/in/rehaan-ashraf-90a8b2278/" target="_blank">LinkedIn</a>

  <br>
  <a href="https://discord.gg/SmXRSbfE">Discord</a>
</body>
</html>
