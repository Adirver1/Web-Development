# Web-Development
/*Check out a dating Web site sample source code. Helpful for beginners learning web development.*/
<!DOCTYPE html>
<html lang="en-US">
    <head>
        <title>HTML Webpage</title>
        <meta charset="utf-8">
        <link rel="stylesheet" href="styles/style.css" media="screen"/>
        <style>
        fieldset{
     background-color:lightyellow;
     border:10px solid yellow;
     margin-bottom:10px;
     width:720px;
}
label{
    
    text-align: right;
    
    display: inline-block;
    width:180px;
}
label:hover { font-size:40px }

textarea{
    width: 360px;
    height: 50px;
}
#methodsofcontact{
    width:auto;
}
.indi{
    position:relative; top:-10px;
    background-color:red;
}
        </style>
    </head>
    <body>
        <h1>Please Enter your details for our dating website!!</h1>
        <form action=" https://ihome.ust.hk/~rossiter/cgi-bin/show_everything.php" method="POST" enctype="multipart/form-data">
        <fieldset>
            <legend>Your Face</legend>
            <label for="avatar">Your Image:</label>
            <input type="file" id="avatar" name="avatar" required="required" /><br/>
            Image perview:
            <img id="preview"/>
        </fieldset>
        <fieldset>
            <legend>Your General Details</legend>
            <label for="Name">Name:</label>
            <input type="text" name="name" required="required" placeholder="Enter your full name here" id="name"/><br/>
            <label for="Gender">Gender:</label>
            Male <input type="radio" name="gender" id="male"/>
            Female <input type="radio" name="gender" id="female" /><br/>
            <label for="Age">Age:</label>
            <input type="number" value="18" required="required" name="age"/><br/>
            <label for="DOB">Date of Birth:</label>
            <input type="date" name="date" required/><br/>
            <label for="Favouritecolor">Favourite Color:</label>
            <input type="color" name="color" required/><br/>
            <label for="country">Nationality:</label>
            <select name="nationalities">
                <option value="ind">Indian</option>
                <option value="chn">Chinese</option>
                <option value="rus">Russian</option>
                <option value="aus">Australian</option>
                <option value="esp">Spanish</option>
                <option value="no">None of the above</option> 
                </select><br/> 
        </fieldset>
        <fieldset>
            <legend>Your Indicators</legend>
            <label for="height">Height:</label>
           <span class="indi">Short</span><input type="range" min="0" max="100" step="5" value="50" id="height" name="height"/><span class="indi" >Tall</span><br/>
            <label for="salary">Salary:</label>
            <span class="indi" >Low</span><input type="range" min="0" max="100" step="5" value="50" id="salary" name="salary"/><span class="indi" >High</span><br/>
        </fieldset>
        <fieldset>
             <legend>Your Contact Information</legend>
             <label for="emailaddress">Email:</label>
             <input type="email" name="email" id="email" required/><br/>
             <label for="mobilenumber">Mobile No.</label>
             <input type="number" name="number" id="mobilenumber" required/><br/>
             <label for="Address"><div id="address">Address:</div></label>
             <textarea rows="3" cols="60" name="Address">
                 Please enter your Address here
             </textarea><br/>
             <label for="methodsofcontact">Methods Of Contact</label>
             Email:<input type="checkbox" name="email" id="methodsofcontact" required/>
             Whatsapp:<input type="checkbox" name="whatsapp" id="methodsofcontact" required/>
             In-appchat:<input type="checkbox" name="inappachat" id="methodsofcontact" required/> 
        </fieldset>
        <input type="submit" value="Submit">
        </form>
<script src="https://www.cse.ust.hk/~rossiter/dating_web_site.js"></script>
    </body>
</html>
