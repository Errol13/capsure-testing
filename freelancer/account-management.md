# Freelancer Account Management - Manual Test Cases

## Related User Story:
1. As a freelancer, I want to be able to create an account and log in using the credentials entered so I can use the application and start my career as a freelancer.
2. As a freelancer, I want to reset my password so I can recover my account when I forgot the password.

--- 
## TC_FRLNCR_001a: Register with valid inputs
- **Preconditions**: None
- **Steps** :
    1. Go to Sign Up Page
    2. Enter valid name, email and 8-length password
    3. Click "Sign Up"
- **Expected Result**: Account is created and freelancer is redirected to their dashboard.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_001b: Register with invalid inputs
- **Preconditions**: None
- **Steps** :
    1. Go to Sign Up Page
    2. Enter invalid email format, less than 8 characters password or leave a field blank.
    3. Click "Sign Up"
- **Expected Result**: Error or validation message appears; "invalid email format", "password must be at least 8 characters" or "required field is missing"
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_002a: Login with valid credentials 
- **Preconditions**: Freelancer account is already registered.
- **Steps** :
    1. Go to Login Page
    2. Enter correct email and password
    3. Click "Login"
- **Expected Result**: Freelancer is logged in successfully and redirected to their dashboard.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_002b: Login with invalid credentials
- **Preconditions**: Freelancer account exists.
- **Steps** :
    1. Go to Login Page
    2. Enter invalid email format, incorrect password or leave a field blank
    3. Click "Login"
- **Expected Result**: Error message shown; freelancer is not logged in. 
- **Status**:
    - [ ] Pass 
    - [ ] Fail 

--- 
## TC_FRLNCR_003: Reset Password 
- **Preconditions**: Freelancer must have a registered email.
- **Steps** :
    1. Click "Forgot Password" in the Login Page
    2. Enter the registered email 
    3. Click "Submit"
    4. Check email inbox for reset instructions.
- **Expected Result**: Password reset email is received successfully.
- **Status**:
    - [ ] Pass 
    - [ ] Fail
