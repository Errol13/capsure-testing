# Client Account Management - Manual Test Cases

## Related User Story:
1. As a client, I want to be able to create an account and log in using my credentials so that I can start hiring freelancers for my needs.
2. As a client, I want to reset my password so I can recover my account when I forgot the password.

--- 
## TC_CLNT_001a: Register with valid inputs
- **Preconditions**: None
- **Steps** :
    1. Go to Sign Up Page
    2. Enter valid name, email and 8-length password
    3. Click "Sign Up"
- **Expected Result**: Account is created and client is redirected to their dashboard.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_CLNT_001b: Register with invalid inputs
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
## TC_CLNT_002a: Login with valid credentials 
- **Preconditions**: Client account is already registered.
- **Steps** :
    1. Go to Login Page
    2. Enter correct email and password
    3. Click "Login"
- **Expected Result**: Client is logged in successfully and redirected to their dashboard.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_CLNT_002b: Login with invalid credentials
- **Preconditions**: Client account exists.
- **Steps** :
    1. Go to Login Page
    2. Enter invalid email format, incorrect password or leave a field blank
    3. Click "Login"
- **Expected Result**: Error message shown; client is not logged in. 
- **Status**:
    - [ ] Pass 
    - [ ] Fail 

--- 
## TC_CLNT_003: Reset Password 
- **Preconditions**: Client must have a registered email.
- **Steps** :
    1. Click "Forgot Password" in the Login Page
    2. Enter the registered email 
    3. Click "Submit"
    4. Check email inbox for reset instructions.
- **Expected Result**: Password reset email is received successfully.
- **Status**:
    - [ ] Pass 
    - [ ] Fail
