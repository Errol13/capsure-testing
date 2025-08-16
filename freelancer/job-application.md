# Freelancer Job Application Processs - Manual Test Cases

## Related User Story:
1. As a freelancer, I want to see all the existing job posts related to my profession so that I can apply to them.
2.  As a freelancer, I want to see all the clients’ requests who want to avail of my service so that I can accept or
decline their requests.


--- 
## TC_FRLNCR_009a: Register with valid inputs
- **Preconditions**: Freelancer is logged in and in their homepage.
- **Steps** :
    1. Observe the list of available job posts
- **Expected Result**: All existing job posts are displayed. If no job exists, "No available jobs" is shown.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_009b: Search Job Posts
- **Preconditions**: Freelancer is logged in and in their homepage.
- **Steps** :
    1. Click the search bar
    2. Enter a service or name of the client
    3. Click "Enter" or click the search button
- **Expected Result**: Job posts with matching service or client name are displayed. If nothing matches, displays "No job posts found".
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_009c: Filter Job Posts by Profession
- **Preconditions**: Freelancer is logged in and in their homepage.
- **Steps** :
    1. Click the filter icon beside the search button
    2. Click the "service" field and select a profession
    3. Click "Ok" to apply the filter
- **Expected Result**: Only job posts relevant to the profession selected are displayed. If nothing matches, displays "No job posts found".
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_0010a: Apply to Job Post with Matching Service
- **Preconditions**: 
    - Freelancer is logged in and in their homepage.
    - Freelancer has a matching service to job post (e.g. Job Post need videographer, freelancer should be offering videographer service).
- **Steps** :
    1. Select one job post and click "View Details"
    2. Click "Apply Job" 
    3. Click the "Select Available Job" field and select one job
    4. The "Apply as a/an" field should be automatically selected
    5. Click "Confirm Application" button to submit.
- **Expected Result**: Job Application was submitted successfully and a dialog box showing application success is shown. 
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_0010b: Apply to Job Post without Matching Service
- **Preconditions**: 
    - Freelancer is logged in and in their homepage.
    - Freelancer does not have a matching service to the job post (e.g. Job Post needs videographer, freelancer only offers graphic design).
- **Steps** :
    1. Select one job post and click "View Details"
    2. Click "Apply Job" 
    3. Click the "Select Available Job" field and select one job
- **Expected Result**: "Apply as a/an" will display "No matching service"; "Confirm Application" button is still disabled. No application is submitted.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 