# SignIn-page-Website
Front-End Design for Signin page

 ---Sign-up File ------- sigup.html
 <!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Registration Form</title>
    <link rel="stylesheet" type="text/css" href="ss.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.2/css/fontawesome.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<style type="text/css">
    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-size: 14px;
    background: #f2f2f2;
}
.container {
    background: white;
    max-width: 500px; /* Adjusted to max-width for responsiveness */
    padding: 25px;
    margin: 50px auto 0;
    border-top: solid blue 4px;
    box-shadow: rgba(0, 0, 0, 0.16) 0px 3px 6px, rgba(0, 0, 0, 0.23) 0px 3px 6px;
}

.container h1 {
    font-size: 24px;
    line-height: 24px;
    padding-bottom: 30px;
    text-align: center;
}

.form-container {
    width: 100%;
}

.input-name {
    width: 90%;
    position: relative;
    margin: 20px auto;
}

.lock {
    padding: 8px 11px;
    color: blue;
    font-size: 14px;
}

.name {
    width: 45%;
    padding: 8px 0px 8px 40px;
}

.input-name span {
    margin-left: 35px;
}

.text-name {
    width: 100%;
    padding: 8px 0px 8px 40px;
}

.input-name i {
    position: absolute;
    font-size: 18px;
    border-right: 1px solid #cccccc;
    color: blue;
}

.text-name,
.name {
    border: 1px solid #cccccc;
    outline: none;
    -webkit-transition: all 0.30s ease-in-out;
    -moz-transition: all 0.30s ease-in-out;
    -ms-transition: all 0.30s ease-in-out;
    transition: all 0.30s ease-in-out;
}

.name:hover,
.text-name:hover {
    background-color: #ffffff;
}

.name:focus,
.text-name:focus {
    border: 1px solid blue;
}

.radio-button {
    margin-right: 5px;
}

.country {
    display: inline-block;
    width: 100%;
    height: 35px;
    padding: 0px 15px;
    cursor: pointer;
    border: 1px solid #cccccc;
    color: #7b7b7b;
    background-color: white;
    appearance: none;
    -webkit-appearance: none;
    -moz-appearance: none;
    transition: all 0.2s ease;
}

.country ::ms-expand {
    display: none;
}

.country:hover,
.country:focus {
    color: blue;
    background: #fafafa;
    border-color: blue;
    outline: none;
}

.arrow {
    position: absolute;
    top: calc(50% - 4px);
    right: 15px;
    width: 0;
    height: 0;
    pointer-events: none;
    border-width: 8px 5px 0px 5px;
    border-style: solid;
    border-color: #7b7b7b transparent transparent transparent;
}

.country:hover + .arrow,
.country:focus + .arrow {
    border-top-color: blue;
}

.submit-button {
    background-color: blue;
    color: white;
    font-size: 18px;
    height: 35px;
    width: 100%;
    line-height: 35px;
    border: none;
    outline: none;
    cursor: pointer;
    margin-bottom: 10px;
}

.submit-button:hover {
    background: green;
}

.signin-options {
    text-align: center;
    margin-top: 20px;
}

.signin-options p {
    margin-bottom: 10px;
}

.signin-options a {
    color: blue;
    text-decoration: none;
}

.signin-options a:hover {
    text-decoration: underline;
}

@media (max-width: 480px) {
    .container {
        width: 100%;
        padding: 5px;
    }
    .input-name {
        margin-bottom: -10px;
    }
    .name {
        width: 100%;
        padding: 8px 0px 8px 40px;
        margin-bottom: 10px;
    }
    .input-name span {
        padding: 0;
        margin: 0;
    }
}
</style>
<body>
    <div class="container">
        <h1>Registration Form</h1>
        <div class="form-container">
            <form>
                
                <div class="input-name">
                    <i class="fa fa-user lock"></i>
                    <input type="text" placeholder="First Name" class="name" name="firstName">
                    <span>
                        <i class="fa fa-user lock"></i>
                        <input type="text" placeholder="Last Name" class="name" name="lastName">
                    </span>
                </div>

                <div class="input-name">
                    <i class="fa fa-envelope lock"></i>
                    <input type="email" placeholder="Email" class="text-name" name="email">
                </div>

                <div class="input-name">
                    <i class="fa fa-unlock-alt lock"></i>
                    <input type="password" placeholder="Password" class="text-name" name="password">
                </div>

                <div class="input-name">
                    <i class="fa fa-unlock-alt lock"></i>
                    <input type="password" placeholder="Confirm Password" class="text-name" name="confirmPassword">
                </div>

                <div class="input-name">
                    <input type="radio" class="radio-button" name="gender" value="male"> <label style="margin-right: 30px;">Male</label>
                    <input type="radio" class="radio-button" name="gender" value="female"> <label>Female</label>
                </div>

                <div class="input-name">
                    <select class="country" name="country">
                        <option>Select a country</option>
                        <option>India</option>
                        <option>China</option>
                        <option>Nepal</option>
                        <option>Italy</option>
                        <option>Maldives</option>
                    </select>
                    <div class="arrow"></div>
                </div>

                <div class="input-name">   
                    <input type="checkbox" class="check-button">
                    <label for="check-button">I accept terms and conditions</label> 
                </div>

                <div class="input-name">
                    <input type="submit" class="submit-button" value="Register">
                </div>

                <div class="signin-options">
                    <p>Already have an account? <a href=" signin.html">Sign In</a></p>
                    <p>Want to explore without signing up? <a href="continueasguest.html">Continue as guest</a></p>
                </div>

            </form>
        </div>
    </div>

    <!-- JavaScript for form validation could go here -->

</body>
</html>


---------sign in File ------sign.html-------

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign In</title>
    <link rel="stylesheet" href="ss.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.2/css/fontawesome.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        /* Additional or overriding styles specific to sign-in page */
        body {
            font-size: 14px;
            background: #f2f2f2;
        }
        .container {
            max-width: 500px;
            padding: 25px;
            margin: 50px auto 0;
            border-top: solid blue 4px;
            box-shadow: rgba(0, 0, 0, 0.16) 0px 3px 6px, rgba(0, 0, 0, 0.23) 0px 3px 6px;
            background: white;
        }
        .container h1 {
            font-size: 24px;
            line-height: 24px;
            padding-bottom: 30px;
            text-align: center;
        }
        .input-name {
            width: 90%;
            position: relative;
            margin: 20px auto;
        }
        .input-name i {
            position: absolute;
            top: 50%;
            left: 10px;
            transform: translateY(-50%);
            color: blue;
            font-size: 14px;
        }
        .text-name {
            width: 100%;
            padding: 8px 0px 8px 40px;
            border: 1px solid #cccccc;
            outline: none;
            -webkit-transition: all 0.30s ease-in-out;
            -moz-transition: all 0.30s ease-in-out;
            -ms-transition: all 0.30s ease-in-out;
            transition: all 0.30s ease-in-out;
        }
        .text-name:hover,
        .text-name:focus {
            border: 1px solid blue;
            background-color: #ffffff;
        }
        .submit-button {
            background-color: blue;
            color: white;
            font-size: 18px;
            height: 35px;
            width: 100%;
            line-height: 35px;
            border: none;
            outline: none;
            cursor: pointer;
            margin-top: 10px;
        }
        .submit-button:hover {
            background: green;
        }
        .forgot-password {
            text-align: right;
            margin-top: 10px;
        }
        .forgot-password a {
            color: blue;
            text-decoration: none;
        }
        .forgot-password a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Sign In</h1>
        <div class="form-container">
            <form>
                <div class="input-name">
                    <i class="fa fa-user"></i>
                    <input type="text" placeholder="Username" class="text-name" name="username">
                </div>

                <div class="input-name">
                    <i class="fa fa-unlock-alt"></i>
                    <input type="password" placeholder="Password" class="text-name" name="password">
                </div>

                <div class="forgot-password">
                    <a href="#">Forgot Password?</a>
                </div>

                <div class="input-name">
                    <input type="submit" class="submit-button" value="Sign In">
                </div>
            </form>
        </div>
    </div>
</body>
</html>


-----------continue as guest file ------continueasguest.html-------


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign In</title>
    <link rel="stylesheet" href="ss.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.2/css/fontawesome.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        /* Additional or overriding styles specific to sign-in page */
        body {
            font-size: 14px;
            background: #f2f2f2;
        }
        .container {
            max-width: 500px;
            padding: 25px;
            margin: 50px auto 0;
            border-top: solid blue 4px;
            box-shadow: rgba(0, 0, 0, 0.16) 0px 3px 6px, rgba(0, 0, 0, 0.23) 0px 3px 6px;
            background: white;
        }
        .container h1 {
            font-size: 24px;
            line-height: 24px;
            padding-bottom: 30px;
            text-align: center;
        }
        .input-name {
            width: 90%;
            position: relative;
            margin: 20px auto;
        }
        .input-name i {
            position: absolute;
            top: 50%;
            left: 10px;
            transform: translateY(-50%);
            color: blue;
            font-size: 14px;
        }
        .text-name {
            width: 100%;
            padding: 8px 0px 8px 40px;
            border: 1px solid #cccccc;
            outline: none;
            transition: all 0.30s ease-in-out;
        }
        .text-name:hover,
        .text-name:focus {
            border: 1px solid blue;
            background-color: #ffffff;
        }
        .submit-button {
            background-color: blue;
            color: white;
            font-size: 18px;
            height: 35px;
            width: 100%;
            line-height: 35px;
            border: none;
            outline: none;
            cursor: pointer;
            margin-top: 10px;
        }
        .submit-button:hover {
            background: green;
        }
        .forgot-password {
            text-align: right;
            margin-top: 10px;
        }
        .forgot-password a {
            color: blue;
            text-decoration: none;
        }
        .forgot-password a:hover {
            text-decoration: underline;
        }
        .guest-button {
            background-color: green;
            color: white;
            font-size: 18px;
            height: 35px;
            width: 100%;
            line-height: 35px;
            border: none;
            outline: none;
            cursor: pointer;
            margin-top: 10px;
        }
        .guest-button:hover {
            background: darkgreen;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Continue as Guest</h1>
        <div class="form-container">
            <form method="POST" action="/signin">
                <div class="input-name">
                    <i class="fa fa-user"></i>
                    <input type="text" placeholder="Temporary Username" class="text-name" name="username" required>
                </div>

                <div class="input-name">
                    <i class="fa fa-envelope"></i>
                    <input type="email" placeholder="Email" class="text-name" name="email">
                </div>

                <div class="forgot-password">
                    <a href="#">Forgot Password?</a>
                </div>

                
            </form>
            <form method="POST" action="/guest">
                <div class="input-name">
                    <input type="submit" class="guest-button" value="Continue as Guest">
                </div>
            </form>
        </div>
    </div>
</body>
</html>
