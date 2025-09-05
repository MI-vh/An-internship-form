<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CNPS Internship Application Form</title>
  <link rel="icon" href="https://www.cnps.cm/images/sampledata/logo-cnps-2024-actualise-1.jpg" alt="CNPS LOGO">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #005baa;
      color: white;
      padding: 20px;
      text-align: center;
    }

    main {
      padding: 30px;
      max-width: 800px;
      margin: auto;
      background-color: white;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h2 {
      color: #005baa;
      margin-bottom: 20px;
    }

    form {
      display: grid;
      gap: 15px;
    }

    label {
      font-weight: bold;
      margin-top: 10px;
    }

    input, select, textarea {
      padding: 10px;
      font-size: 1em;
      border: 1px solid #ccc;
      border-radius: 5px;
      width: 100%;
    }
#otherField {
  padding: 10px;
  border-radius: 5px;
  border:  1px solid#ccc;
  width: 100%;
  max-width: 300px;
}

.gender-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  margin: 5px;
  padding: 12px 24px;
  font-size: 1rem;
  border: none;
  background-color: #007BFF;
  color: white;
  border-radius: 25px;
  cursor: pointer;
  transition: background-color 0.5s ease;
  width: 100%;
  max-width: 200px;

   }
 .gender-btn.active{
   background-color: #0056b3;
   box-shadow: 0 0 10px rgba(0, 123, 255, 0.5);
   }

.internshiptype-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  margin: 5px;
  padding: 12px 24px;
  font-size: 1rem;
  border: none;
  background-color: #007BFF;
  color: white;
  border-radius: 25px;
  cursor: pointer;
  transition: background-color 0.5s ease;
  width: 100%;
  max-width: 200px;

   }
 .internshiptype-button.active {
   background-color: #0056b3;
   box-shadow: 0 0 10px rgba(0, 123, 255, 0.5);

}

   button {
      background-color: #005baa;
      color: white;
      padding: 13px;
      border: none;
      border-radius: 25px;
      font-size: 2em;
      cursor: pointer;
      margin-top: 20px;
      width: 350px;
    }

    button:hover {
      background-color: #004080;
    }

    fieldset {
      border: none;
      border-radius: 8px;
      padding: 20px;
      margin-top: 20px;
    }

    legend {
      font-weight: bold;
      color: #005baa;
      padding: 0 10px;
    }

    .other-input {
      display: none;
      margin-top: 10px;
    }

  .error {
  color: red;
 font-size: 0.9em;
 display: none;
margin-bottom: 10px;
}
.active{
background-color: #d0eaff;
border: 2px solid #007bff;



}

    .checkbox-group {
      display: flex;
      margin-bottom: 8px;
      
    }

   
     #confirmationMessage {
  background-color: #e6ffe6;
  border: 1px solid #00cc00;
  padding: 15px;
  font-weight: bold;
  margin-top: 20px;
}

    footer {
      background-color: #003d73;
      color: white;
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <img src="https://www.cnps.cm/images/sampledata/logo-cnps-2024-actualise-1.jpg" alt="CNPS Logo" style="height: 80px;">
    <h1>CNPS Internship Application Form</h1>
    <p>Apply for an internship opportunity with CNPS Cameroon</p>
  </header>

<main>
  <h2>Applicant Information</h2>
  <form id="internshipForm">

    <label for="fullName">Full Name</label>
    <input type="text" id="fullName" name="fullName" required />
    <span class="error" id="errorFullName">Full name is required.</span>

    <label for="dob">Date of Birth</label>
    <input type="date" id="dob" name="dob" required />
    <span class="error" id="errorDob">Date of birth is required.</span>

    <label>Gender</label>
    <button type="button" class="gender-btn" data-gender="Male">👨 Male</button>
    <button type="button" class="gender-btn" data-gender="Female">👩 Female</button>
    <span class="error" id="errorGender">Gender is required.</span>

    <label for="email">Email Address</label>
    <input type="email" id="email" name="email" required />
    <span class="error" id="errorEmail">Valid email is required.</span>

    <label for="phone">Phone Number</label>
    <input type="number" id="phone" name="phone" required />
    <span class="error" id="errorPhone">Phone number is required.</span>

    <label for="address">Residential Address</label>
    <textarea id="address" name="address" rows="3" required></textarea>
    <span class="error" id="errorAddress">Enter your address here.</span>

    <h2>Academic Information</h2>

    <label for="institution">Institution Name</label>
    <input type="text" id="institution" name="institution" required />
    <span class="error" id="errorfod">Institution name is required.</span>

    <label for="field">Field of Study</label>
    <select id="field" name="field" class="dropdown">
      <option value="science">Natural Sciences</option>
      <option value="engineering">Engineering & Tech</option>
      <option value="arts">Arts</option>
      <option value="business">Business</option>
      <option value="others">Other</option>
    </select>

    <div id="otherfieldcontainer" style="display: none; margin-top: 10px;">
      <label for="otherfield">Please specify:</label>
      <input type="text" id="otherfield" name="otherfield" placeholder="Enter your field of study!" />
      <span class="error" id="errorOtherField">Field of study is required.</span>
    </div>

    <label for="level">Current Level</label>
    <select id="level" name="level" required>
      <option value="">Select</option>
      <option value="First year">First year</option>
      <option value="Second year">Second year</option>
      <option value="Third year">Third year</option>
      <option value="Fourth year">Fourth year</option>
      <option value="Fifth year">Fifth year</option>
      <option value="Bachelor">Bachelor</option>
      <option value="Master">Master</option>
      <option value="PhD">PhD</option>
      <option value="Other">Other</option>
    </select>
    <span class="error" id="errorLevel">Enter your current level.</span>

    <label for="academicsupervisor">Academic Supervisor</label>
    <input type="text" id="academicsupervisor" name="supervisor" required />
    <span class="error" id="erroracademicsupervisor">Enter your academic supervisor.</span>

    <h2>Skills & Competencies</h2>
    <div class="checkbox-group">
      <label><input type="checkbox" name="skills[]" value="Communication"> Communication</label>
      <label><input type="checkbox" name="skills[]" value="Teamwork"> Teamwork</label>
      <label><input type="checkbox" name="skills[]" value="Problem Solving"> Problem Solving</label>
      <label><input type="checkbox" name="skills[]" value="Technical Knowledge"> Technical Knowledge</label>
      <label><input type="checkbox" name="skills[]" value="Other"> Other</label>
      <span class="error" id="errorskills">Select at least one skill.</span>
    </div>

    <div class="other-input" id="otherSkillInput">
      <label for="otherText">Please specify:</label>
      <input type="text" id="otherText" name="otherSkillText" placeholder="Your skill..." />
      <span class="error" id="errorother">Enter your skill if not listed.</span>
    </div>

    <h2>Motivation</h2>
    <label for="motivation">Why do you want to intern at CNPS?</label>
    <textarea id="motivation" name="motivation" rows="5" placeholder="Share your motivation..." required></textarea>
    <span class="error" id="errormotivation">Motivation is required.</span>

    <h2>Internship Date</h2>
    <label for="internshipPeriod">Preferred Internship Period</label>
    <input type="text" id="internshipPeriod" name="internshipPeriod" placeholder="e.g., June 2025 – August 2025" />

    <h2>Internship Type</h2>
    <label><button type="button" class="internshiptype-button" data-type="Academic">Academic</button></label>
    <label><button type="button" class="internshiptype-button" data-type="Professional">Professional</button></label>
    <label><button type="button" class="internshiptype-button" data-type="Holiday">Holiday</button></label>
    <label><button type="button" class="internshiptype-button" data-type="Voluntary">Voluntary</button></label>
    <span class="error" id="errortype">Select an internship type.</span>

    <h2>Upload Documents</h2>
    <label for="documents">Upload Resume and Cover Letter</label>
    <input type="file" id="documents" name="documents[]" multiple accept=".pdf,.doc,.docx" />
    <span class="error" id="errordocs">Upload your documents.</span>

    <button type="submit">Submit Application</button>
  </form>

  <div id="confirmationMessage" style="display: none;">✅ Your internship application has been submitted successfully!</div>
</main>

<footer>
  <p>&copy; 2025 CNPS Cameroon — All rights reserved.</p>
  The Caisse Nationale de Prévoyance Sociale (CNPS) in Cameroon has multiple branches across the country. The main headquarters is located at:<br>
  📍 Place de l'Indépendance, Yaoundé, Cameroon<br>
  📞 Phone: (+237) 222 22 46 01<br>
  📧 Email: cnps.cameroun@cnps.cm<br>
  🕒 Hours: Monday to Friday, 7:30 AM – 3:30 PM
</footer>
    

<script>
document.querySelectorAll('.error').forEach(elem => {
  elem.style.display = 'none';
});

const form = document.getElementById('internshipForm');
  const confirmationMessage = document.getElementById('confirmationMessage');

  form.addEventListener('submit', function (e) {
    e.preventDefault();
    let isValid = true;

   
    function toggleError(id, condition) {
      const errorElem = document.getElementById(id);
      errorElem.style.display = condition ? "block" : "none";
      if (condition) isValid = false;
    }

    
    const requiredFields = [
      { id: "fullName", errorId: "errorFullName" },
       { id: "dob", errorId: "errorDob" },
      { id: "email", errorId: "errorEmail" },
      { id: "phone", errorId: "errorPhone" },
      { id: "address", errorId: "errorAddress" },
      { id: "institution", errorId: "errorfod" },
      { id: "level", errorId: "errorLevel" },
      { id: "academicsupervisor", errorId: "erroracademicsupervisor" },
      { id: "motivation", errorId: "errormotivation" }
    ];

    requiredFields.forEach(field => {
      const value = document.getElementById(field.id).value.trim();
      toggleError(field.errorId, value === "");
    });

    
const genderButtons = document.querySelectorAll(".gender-btn");
    let genderSelected = false;
    genderButtons.forEach(btn => {
      if (btn.classList.contains("active")) genderSelected = true;
    });
    toggleError("errorGender", !genderSelected);

    
    const field = document.getElementById("field").value;
    if (field === "others") {
      const otherField = document.getElementById("otherfield").value.trim();
      toggleError("errorOtherField", otherField === "");
    }

    
    const skills = document.querySelectorAll("input[name='skills[]']:checked");
    toggleError("errorskills", skills.length === 0);

const otherSkillChecked = [...skills].some(skill => skill.value === "Other");
    const otherSkillInput = document.getElementById("otherText").value.trim();
    if (otherSkillChecked) {
      toggleError("errorother", otherSkillInput === "");
    }

    
    const typeButtons = document.querySelectorAll(".internshiptype-button");
    let typeSelected = false;
    typeButtons.forEach(btn => {
      if (btn.classList.contains("active")) typeSelected = true;
    });
    toggleError("errortype", !typeSelected);
 const documents = document.getElementById("documents").files;
    toggleError("errordocs", documents.length === 0);

    
    if (isValid) {
      confirmationMessage.style.display = 'block';
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  });

  
  const genderButtons = document.querySelectorAll('.gender-btn');
  genderButtons.forEach(button => {
    button.addEventListener('click', () => {
      genderButtons.forEach(btn => btn.classList.remove('active'));
      button.classList.add('active');
    });
 });

  
  const internshipButtons = document.querySelectorAll('.internshiptype-button');
  internshipButtons.forEach(button => {
    button.addEventListener('click', () => {
      internshipButtons.forEach(btn => btn.classList.remove('active'));
      button.classList.add('active');
    });
  });
 document.getElementById('field').addEventListener('change', () => {
    const otherContainer = document.getElementById('otherfieldcontainer');
    otherContainer.style.display = document.getElementById('field').value === 'others' ? 'block' : 'none';
  });
</script>
