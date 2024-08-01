# HTML-Portfolio-Form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Forms using HTML</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 400px;
            max-height: 90vh;
            overflow-y: auto;
        }
        .form-container::-webkit-scrollbar {
            width: 10px;
        }
        .form-container::-webkit-scrollbar-thumb {
            background-color: #ccc;
            border-radius: 5px;
        }
        .form-container::-webkit-scrollbar-track {
            background-color: #f4f4f9;
        }
        h2 {
            color: #333;
            text-align: center;
        }
        label {
            display: block;
            margin-bottom: 10px;
            font-weight: bold;
            color: #555;
        }
        input[type="text"], 
        input[type="email"], 
        input[type="date"], 
        input[type="number"], 
        input[type="password"], 
        textarea, 
        select {
            width: 100%;
            padding: 10px;
            margin: 5px 0 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input[type="radio"], input[type="checkbox"] {
            margin-right: 10px;
        }
        input[type="submit"], input[type="reset"] {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            margin: 10px 5px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            width: calc(50% - 15px);
        }
        input[type="submit"]:hover, input[type="reset"]:hover {
            background-color: #45a049;
        }
        div {
            margin-bottom: 15px;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <form action="data.sql">
            <h2><u>Portfolio Form (by ALOK) </u></h2>
            
            <div>
                <label for="name">Name:</label>
                <input type="text" placeholder="Enter name" name="myName" id="name">
            </div>
            
            <div>
                <label for="jobRole">Job Role:</label>
                <input type="text" placeholder="Enter job role" name="myJobRole" id="jobRole">
            </div>
            
            <div>
                <label for="email">Email:</label>
                <input type="email" placeholder="Enter email" name="myEmail" id="email">
            </div>
            
            <div>
                <label for="dob">D.O.B:</label>
                <input type="date" name="myDob" id="dob">
            </div>
            
            <div>
                <label>Gender:</label>
                <input type="radio" name="myGender" value="male" id="male"> 
                <label for="male">Male</label>
                <input type="radio" name="myGender" value="female" id="female"> 
                <label for="female">Female</label>
                <input type="radio" name="myGender" value="other" id="other"> 
                <label for="other">Other</label>
            </div>
            
            <div>
                <label for="experience">Experience:</label>
                <input type="number" placeholder="In years" name="myExperience" id="experience">
            </div>
            
            <div>
                <label for="eligibility">Are you eligible?</label>
                <input type="checkbox" name="myEligibility" id="eligibility" checked>
            </div>
            
            <div>
                <label for="myFeedback">Feedback Section:</label>
                <textarea name="myFeedback" placeholder="Give feedback" id="myFeedback" cols="30" rows="4"></textarea>
            </div>
            
            <div>
                <label for="password">Password:</label>
                <input type="password" name="myPassword" placeholder="Enter password" id="password">
            </div>
            
            <div>
                <label for="state">Select your state:</label>
                <select name="myState" id="state">
                    <option value="delhi">Delhi</option>
                    <option value="maharashtra">Maharashtra</option>
                    <option value="punjab">Punjab</option>
                    <option value="bihar">Bihar</option>
                    <option value="up">Uttar Pradesh</option>
                    <option value="jammu-kashmir">Jammu & Kashmir</option>
                    <option value="bangalore">Bangalore</option>
                    <option value="others" selected>Other State</option>
                </select>
            </div>
            
            <div>
                <input type="submit" value="Submit Information">
                <input type="reset" value="Reset Information">
            </div>
        </form>
    </div>
</body>
</html>
