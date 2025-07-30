# Admin Account Management - Manual Test Cases

## Related User Story:
1. As an admin, I want to login so that I can access the admin dashboard.

--- 
## TC_ADMN_001a: Login with valid credentials
- **Preconditions** : Administrator account is provided and registered to the system.
- **Steps**: 
   1. Go to Admin Login Page by accessing the homepage url with "/admin"
   2. Enter valid username/email and password.
   3. Click "Login"
- **Expected Result**: Admin is logged in successfully and redirected to the admin dashboard.
- **Status**: 
    - [ ] Pass
    - [ ] Fail

--- 
## TC_ADMN_001b: Login with invalid credentials
- **Preconditions** : Administrator account is provided and registered to the system.
- **Steps**: 
   1. Go to Admin Login Page by accessing the homepage url with "/admin"
   2. Enter either invalid username/email or password.
   3. Click "Login"
- **Expected Result**: Error shown and admin is not logged in.
- **Status**: 
    - [ ] Pass
    - [ ] Fail
