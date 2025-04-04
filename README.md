## Instructions
- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form
>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 # Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.
================================================================================
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>HTML Assignment 2</title>
</head>
<body>
    <header>
        <h1>HTML Elements Example</h1>
        <nav>
            <ul>
                <li><a href="#list-section">Ordered List</a></li>
                <li><a href="#image-section">Image Example</a></li>
                <li><a href="#table-section">Contacts Table</a></li>
                <li><a href="#form-section">Registration Form</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- Ordered List with Roman Numerals -->
        <section id="list-section">
            <h2>Ordered list that uses Roman Numerals</h2>
            <ol type="I">
                <li>Introduction to CSS</li>
                <li>Basic CSS takeaways</li>
                <li>HTML Elements
                    <ol type="a">
                        <li>Text Elements</li>
                        <li>List Elements</li>
                        <li>Table Elements</li>
                    </ol>
                </li>
                <li>HTML Forms</li>
                <li>HTML5 Semantics</li>
            </ol>
        </section>

        <!-- External Image from Pexels -->
        <section id="image-section">
            <h2>Image Example</h2>
            <figure>
                <img src="https://images.pexels.com/photos/30722562" 
                     alt="woman-in-flowing-blue-dress-on-wooden-pier" 
                     width="600">
                <figcaption>Beach recreation. Image source: Pexels</figcaption>
            </figure>
        </section>

        <!-- Contacts Table -->
        <section id="table-section">
            <h2>Contacts Table</h2>
            <table border="1">
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Address</th>
                        <th>Mobile</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>John</td>
                        <td>123 Main St, NY</td>
                        <td>(212) 555-1234</td>
                        <td>john@example.com</td>
                    </tr>
                    <tr>
                        <td>Mary</td>
                        <td>456 Boston</td>
                        <td>(617) 555-5678</td>
                        <td>mary@example.com</td>
                    </tr>
                    <tr>
                        <td>Martha</td>
                        <td>789 Chicago</td>
                        <td>(312) 555-9012</td>
                        <td>martha@example.com</td>
                    </tr>
                    <tr>
                        <td>Simon</td>
                        <td>101 San Francisco</td>
                        <td>(415) 555-3456</td>
                        <td>simon@example.com</td>
                    </tr>
                    <tr>
                        <td>Peter</td>
                        <td>202 Texas</td>
                        <td>(512) 555-7890</td>
                        <td>peter@example.com</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Registration Form -->
        <section id="form-section">
            <h2>Registration Form</h2>
            <form action="#" method="post">
                <!-- Text Fields -->
                <fieldset>
                    <legend>Personal Information</legend>
                    
                    <div>
                        <label for="name">Full Name:</label>
                        <input type="text" id="name" name="name" placeholder="Enter your full name" required>
                    </div>
                    
                    <div>
                        <label for="email">Email Address:</label>
                        <input type="email" id="email" name="email" placeholder="your.email@example.com" required>
                    </div>
                    
                    <div>
                        <label for="password">Password:</label>
                        <input type="password" id="password" name="password" 
                               placeholder="Choose a strong password" 
                               pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" 
                               title="Must contain at least one number, one uppercase and lowercase letter, and at least 8 characters"
                               required>
                    </div>
                    
                    <div>
                        <label for="birthdate">Date of Birth:</label>
                        <input type="date" id="birthdate" name="birthdate" required>
                    </div>
                </fieldset>

                <!-- Dropdown -->
                <fieldset>
                    <legend>Additional Information</legend>
                    
                    <div>
                        <label for="country">Country:</label>
                        <select id="country" name="country">
                            <option value="">Select your country</option>
                            <option value="K">Kenya</option>
                            <option value="UG">Uganda</option>
                            <option value="TZ">Tanzania</option>
                            <option value="NIG">Nigeria</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <!-- Radio Buttons -->
                    <div>
                        <p>Gender:</p>
                        <input type="radio" id="male" name="gender" value="male">
                        <label for="male">Male</label>
                        
                        <input type="radio" id="female" name="gender" value="female">
                        <label for="female">Female</label>
                        
                        <input type="radio" id="non-binary" name="gender" value="non-binary">
                        <label for="non-binary">Non-binary</label>
                        
                        <input type="radio" id="prefer-not" name="gender" value="prefer-not">
                        <label for="prefer-not">Prefer not to say</label>
                    </div>
                    
                    <!-- Checkboxes -->
                    <div>
                        <p>Interests (select all that apply):</p>
                        <input type="checkbox" id="web-dev" name="interests" value="web-dev">
                        <label for="web-dev">Web Development</label>
                        
                        <input type="checkbox" id="design" name="interests" value="design">
                        <label for="design">Graphic Design</label>
                        
                        <input type="checkbox" id="marketing" name="interests" value="marketing">
                        <label for="marketing">Digital Marketing</label>
                        
                        <input type="checkbox" id="data" name="interests" value="data">
                        <label for="data">Data Science</label>
                    </div>
                </fieldset>
                
                <div>
                    <input type="checkbox" id="terms" name="terms" required>
                    <label for="terms">I agree to the terms and conditions</label>
                </div>
                
                <div>
                    <button type="submit">Register</button>
                    <button type="reset">Clear Form</button>
                </div>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 HTML Assignment 2. All rights reserved.</p>
    </footer>
</body>
</html>
