<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration & Search Forms</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="form-container">
        <h2>Student Registration Form</h2>
        <form action="/register" method="post">
            
            <div class="form-group">
                <label for="fullname">Full Name:</label>
                <input type="text" id="fullname" name="fullname">
            </div>

            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
            </div>

            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password">
            </div>

            <div class="form-group">
                <label>Gender:</label>
                <div class="radio-group">
                    <input type="radio" id="male" name="gender" value="male">
                    <label for="male">Male</label>
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Female</label>
                </div>
            </div>

            <div class="form-group">
                <label for="country">Country:</label>
                <select id="country" name="country">
                    <option value="">-- Select Country --</option>
                    <option value="Nigeria">Nigeria</option>
                    <option value="Ghana">Ghana</option>
                    <option value="Kenya">Kenya</option>
                    <option value="South Africa">South Africa</option>
                </select>
            </div>

            <div class="form-group">
                <label for="about">About Yourself:</label>
                <textarea id="about" name="about" rows="4" placeholder="Tell us a little about yourself"></textarea>
            </div>

            <div class="form-group checkbox-group">
                <input type="checkbox" id="terms" name="terms" required>
                <label for="terms">I agree to the terms and conditions</label>
            </div>

            <button type="submit">Register</button>

        </form>
    </div>

    <div class="form-container">
        <h2>Search Website</h2>
        <form action="/search" method="get">
            <div class="form-group search-group">
                <input type="text" name="q" placeholder="Search...">
                <button type="submit">Search</button>
            </div>
        </form>
    </div>

</body>
</html>
