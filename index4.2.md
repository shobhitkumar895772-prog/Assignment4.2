File: job-application.html
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Job Application Form</title>
    <style>
        body { font-family: Arial, sans-serif; background-color: #f4f7f6; margin: 0; padding: 20px; }
        .form-container { background: #ffffff; padding: 30px; border-radius: 8px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); width: 100%; max-width: 600px; margin: auto; }
        h2 { color: #2c3e50; text-align: center; margin-top: 0; margin-bottom: 20px; }
        .form-group { margin-bottom: 18px; }
        label { display: block; margin-bottom: 6px; font-weight: bold; color: #333; }
        input[type="text"], input[type="email"], input[type="tel"], input[type="date"], input[type="url"], select, textarea {
            width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box; font-size: 14px;
        }
        input:focus, select:focus, textarea:focus { border-color: #3498db; outline: none; }
        .radio-group, .checkbox-group { display: flex; gap: 15px; margin-top: 5px; flex-wrap: wrap; }
        .radio-group label, .checkbox-group label { font-weight: normal; display: inline-flex; align-items: center; gap: 5px; cursor: pointer; }
        textarea { resize: vertical; height: 120px; }
        button { width: 100%; background-color: #27ae60; color: white; padding: 12px; border: none; border-radius: 4px; font-size: 16px; font-weight: bold; cursor: pointer; margin-top: 10px; }
        button:hover { background-color: #219653; }
        input:disabled { background-color: #e9ecef; cursor: not-allowed; }
    </style>
</head>
<body>

    <div class="form-container">
        <h2>Job Application Form</h2>
        
        <form action="#" method="POST">
            
            <!-- Disabled Field Example (e.g., Application Status) -->
            <div class="form-group">
                <label for="app-status">Application Status:</label>
                <input type="text" id="app-status" value="Not Submitted" disabled>
            </div>

            <!-- Full Name -->
            <div class="form-group">
                <label for="fullname">Full Name:</label>
                <input type="text" id="fullname" name="fullname" placeholder="John Doe" required>
            </div>

            <!-- Email -->
            <div class="form-group">
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="john.doe@example.com" required>
            </div>

            <!-- Phone -->
            <div class="form-group">
                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" placeholder="123-456-7890" required>
            </div>

            <!-- Date of Birth -->
            <div class="form-group">
                <label for="dob">Date of Birth:</label>
                <input type="date" id="dob" name="dob" required>
            </div>

            <!-- Portfolio URL -->
            <div class="form-group">
                <label for="portfolio">Portfolio URL:</label>
                <input type="url" id="portfolio" name="portfolio" placeholder="https://www.yourportfolio.com">
            </div>

            <!-- Dropdown for Job Role -->
            <div class="form-group">
                <label for="job-role">Applying for Job Role:</label>
                <select id="job-role" name="job_role" required>
                    <option value="">-- Select a Role --</option>
                    <option value="frontend">Front-End Developer</option>
                    <option value="backend">Back-End Developer</option>
                    <option value="fullstack">Full-Stack Developer</option>
                    <option value="uiux">UI/UX Designer</option>
                </select>
            </div>

            <!-- Radio Buttons for Preferred Shift -->
            <div class="form-group">
                <label>Preferred Shift:</label>
                <div class="radio-group">
                    <label><input type="radio" name="shift" value="morning" required> Morning (9 AM - 5 PM)</label>
                    <label><input type="radio" name="shift" value="evening"> Evening (1 PM - 9 PM)</label>
                    <label><input type="radio" name="shift" value="flexible"> Flexible</label>
                </div>
            </div>

            <!-- Checkboxes for Skills -->
            <div class="form-group">
                <label>Technical Skills:</label>
                <div class="checkbox-group">
                    <label><input type="checkbox" name="skills" value="html"> HTML5</label>
                    <label><input type="checkbox" name="skills" value="css"> CSS3</label>
                    <label><input type="checkbox" name="skills" value="js"> JavaScript</label>
                    <label><input type="checkbox" name="skills" value="python"> Python</label>
                </div>
            </div>

            <!-- Textarea for Cover Letter -->
            <div class="form-group">
                <label for="cover-letter">Cover Letter:</label>
                <textarea id="cover-letter" name="cover_letter" placeholder="Tell us why you are a great fit for this role..." required></textarea>
            </div>

            <!-- Submit Button -->
            <button type="submit">Submit Application</button>

        </form>
    </div>

</body>
</html>
Requirements Checklist for Submission:
File Name: Saved as job-application.html.

Personal Info & Inputs: Includes full name, email, phone, date of birth (type="date"), and portfolio (type="url").

Options & Controls: Dropdown <select> for job roles, radio buttons sharing the exact same name="shift", and skill checkboxes.

Textarea & Button: Cover letter textarea included along with a styled submit button.

Rules Met: Every field has a proper <label>, mandatory fields are marked required, and an example of a disabled input field has been added at the top.