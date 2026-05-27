<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roblox - Sign in</title>
    <style>
        /* Base page reset and styling */
        body {
            margin: 0;
            padding: 0;
            background-color: #0b0c10;
            color: #ffffff;
            font-family: "HCo Gotham SSm", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* Centered login panel container */
        .login-container {
            width: 100%;
            max-width: 400px;
            padding: 40px 20px;
            text-align: center;
            box-sizing: border-box;
        }

        /* Top header section */
        h1 {
            font-size: 32px;
            font-weight: 700;
            margin: 0 0 8px 0;
            text-align: left;
        }

        .subtitle {
            font-size: 16px;
            color: #b8b9bd;
            margin: 0 0 32px 0;
            text-align: left;
        }

        /* Form styling */
        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        label {
            display: block;
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 8px;
            color: #ffffff;
        }

        /* Input field container for positioning password visibility icon */
        .input-wrapper {
            position: relative;
            display: flex;
            align-items: center;
        }

        input {
            width: 100%;
            padding: 14px 12px;
            font-size: 16px;
            background-color: #050505;
            border: 1px solid #393b43;
            border-radius: 8px;
            color: #ffffff;
            box-sizing: border-box;
            outline: none;
        }

        input:focus {
            border-color: #ffffff;
        }

        /* Password visibility icon toggle */
        .password-toggle {
            position: absolute;
            right: 12px;
            cursor: pointer;
            width: 20px;
            height: 20px;
            opacity: 0.7;
        }

        /* Action Buttons */
        .btn-primary {
            width: 100%;
            padding: 14px;
            font-size: 16px;
            font-weight: 600;
            background-color: #3965f7;
            color: #ffffff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 12px;
            transition: background-color 0.2s ease;
        }

        .btn-primary:hover {
            background-color: #2a52d4;
        }

        /* Text Links */
        .forgot-link {
            display: inline-block;
            margin-top: 24px;
            margin-bottom: 40px;
            color: #ffffff;
            font-size: 16px;
            font-weight: 600;
            text-decoration: none;
        }

        .forgot-link:hover {
            text-decoration: underline;
        }

        /* Secondary/Alternative Login Options */
        .btn-secondary {
            width: 100%;
            padding: 14px;
            font-size: 15px;
            font-weight: 600;
            background-color: #191b24;
            color: #ffffff;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-bottom: 12px;
            transition: background-color 0.2s ease;
        }

        .btn-secondary:hover {
            background-color: #222530;
        }

        /* Bottom Footer Signup text */
        .signup-text {
            margin-top: 40px;
            font-size: 14px;
            color: #b8b9bd;
        }

        .signup-text a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 600;
            margin-left: 4px;
        }

        .signup-text a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <div class="login-container">
        <h1>Sign in</h1>
        <div class="subtitle">Jump back into your experiences</div>

        <form>
            <!-- Username/Email/Phone Input Field -->
            <div class="form-group">
                <label for="username">Username, email, or phone</label>
                <div class="input-wrapper">
                    <input type="text" id="username" placeholder="Username, email, or phone" autocomplete="username" required>
                </div>
            </div>

            <!-- Password Input Field -->
            <div class="form-group">
                <label for="password">Password</label>
                <div class="input-wrapper">
                    <input type="password" id="password" placeholder="Password" autocomplete="current-password" required>
                    <!-- Visual eye icon placeholder matching the reference screen -->
                    <svg class="password-toggle" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"></path>
                        <circle cx="12" cy="12" r="3"></circle>
                    </svg>
                </div>
            </div>

            <!-- Main Submit Button -->
            <button type="submit" class="btn-primary">Sign in</button>
        </form>

        <!-- Recovery Option -->
        <a href="#" class="forgot-link">Forgot Password or Username?</a>

        <!-- Alternate Entry Methods -->
        <button type="button" class="btn-secondary">Email Me a One-Time Code</button>
        <button type="button" class="btn-secondary">Log In With Another Device</button>

        <!-- Account Creation Navigation Hint -->
        <div class="signup-text">
            Don't have an account?<a href="#">Sign Up</a>
        </div>
    </div>

</body>
</html>
