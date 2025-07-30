# Freelancer Portfolio and Services - Manual Test Cases

## Related User Story:
1. As a freelancer, I want to create a portfolio with photos and videos so I can showcase my credibility.
2. As a freelancer, I want to be able to modify my portfolio so I can share my professional development and improvement.
3. As a freelancer, I want to be able to add services and update my availability status so that clients are informed of any changes.

--- 
## TC_FRLNCR_004a: Create Portfolio with photos and videos
- **Preconditions**: Freelancer should be logged in.
- **Steps** :
    1. Navigate to "Settings" page
    2. Scroll down and click "Create Album"
    3. Enter an "Album Title"
    4. Upload at least one file (image or video)
    5. Verify the preview on the right side
    6. Click "Post"
- **Expected Result**: Album is created successfully with the entered title and uploaded files.
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_004b: Create Portfolio with no file
- **Preconditions**: Freelancer should be logged in.
- **Steps** :
    1. Navigate to "Settings" page
    2. Scroll down and click "Create Album"
    3. Enter an "Album Title"
    4. Do not upload any file
    5. Click "Post"
- **Expected Result**: "Post" button remains disabled. No album is created. 
- **Status**:
    - [ ] Pass 
    - [ ] Fail

---
## TC_FRLNCR_004c: Create Portfolio with no album title
- **Preconditions**: Freelancer should be logged in.
- **Steps** :
    1. Navigate to "Settings" page
    2. Scroll down and click "Create Album"
    3. Leave the "Album Title" field blank
    4. Upload at least one file (image or video)
    5. Click "Post"
- **Expected Result**: Form is not submitted. Validation shows "Please fill out this field".
- **Status**:
    - [ ] Pass 
    - [ ] Fail

--- 
## TC_FRLNCR_005a: Delete all files within an album
- **Preconditions**: 
    - Freelancer is logged in.
    - Freelancer has an existing album with multiple files.
- **Steps**:
    1. Navigate to the "Settings" page
    2. Scroll down to the Portfolios section
    3. Open an existing album with multiple files
    4. Select all files by ticking the circles in the upper-left of each file
    5. Click the "Delete" button located on the right side
    6. Confirm the deletion when prompted
- **Expected Result**: All selected files are deleted. If the album becomes empty, the album itself is also removed.
- **Status**:
    - [ ] Pass  
    - [ ] Fail

--- 
## TC_FRLNCR_005b: Delete an entire album using the dropdown menu
- **Preconditions**: 
    - Freelancer is logged in.
    - Freelancer has at least one existing album.
- **Steps**:
    1. Navigate to the "Settings" page
    2. Scroll down to the Portfolios section
    3. Click the "..." button on the right side of the Portfolios section
    4. Select "Delete Album" from the dropdown menu
    5. Choose the album to delete from the dropdown list
    6. Click "Delete"
    7. Confirm the deletion when prompted
- **Expected Result**: The selected album and all its associated files are deleted successfully.
- **Status**:
    - [ ] Pass  
    - [ ] Fail

---
## TC_FRLNCR_005c: Delete a single file within an album
- **Preconditions**: Freelancer is logged in and has an album with multiple files.
- **Steps**:
    1. Navigate to the "Settings" page
    2. Scroll to the Portfolios section and select an album
    3. Tick the circle in the upper-left corner of one file
    4. Click the "Delete" button located on the right side
    5. Confirm the deletion when prompted
- **Expected Result**: Only the selected file is deleted. The rest of the album remains intact.
- **Status**:
    - [ ] Pass  
    - [ ] Fail
--- 
## TC_FRLNCR_006: Upload files to an existing album
- **Preconditions**: 
    - Freelancer is logged in.
    - Freelancer has an existing album.
- **Steps**:
    1. Navigate to the "Settings" page
    2. Scroll to the Portfolios section
    3. Click the "..." button on the right side of the Portfolios section
    4. Select "Upload Files" from the dropdown
    5. Choose the album where the files will be added
    6. Select one or more files to upload
    7. Click "Update"
- **Expected Result**: The selected files are uploaded and added to the specified album.
- **Postcondition**: The selected album is updated with the new files and saved in the database.
- **Status**:
    - [ ] Pass  
    - [ ] Fail

---

## TC_FRLNCR_007a: Add new service with valid inputs
- **Preconditions**: Freelancer is logged in.
- **Steps**:
    1. Navigate to the "Settings" page.
    2. Scroll down and click the "+" icon beside the Services section.
    3. Fill in the following fields:
        - Job Category (dropdown)
        - Job Title (dropdown or use "Other" for manual input)
        - Job Fee (numeric)
        - Job Type (dropdown)
        - Availability (dropdown)
    4. Click "Add Service".
- **Expected Result**: The new service is added successfully and becomes visible in the Settings or Profile page.
- **Status**:
    - [ ] Pass  
    - [ ] Fail

--- 
## TC_FRLNCR_007b: Attempt to add new service with invalid or incomplete inputs
- **Preconditions**: Freelancer is logged in.
- **Steps**:
    1. Navigate to the "Settings" page.
    2. Scroll down and click the "+" icon beside the Services section.
    3. Leave one or more of the following fields blank or provide invalid input:
        - Job Category (leave blank)
        - Job Title (leave blank)
        - Job Fee (enter non-numeric input)
        - Job Type (leave blank)
    4. Click "Add Service".
- **Expected Result**: Form submission is blocked. Validation errors are displayed, such as:
    - "Please select an item from the list."
    - "Job Title is a required field."
    - "Job Fee must be a number."
- **Status**:
    - [ ] Pass  
    - [ ] Fail

---
## TC_FRLNCR_008: Modify an existing service
- **Preconditions**: 
    - Freelancer is logged in.
    - At least one service exists in the freelancer's profile.

- **Steps**:
    1. Navigate to the "Settings" page.
    2. Scroll down to the Services section and click the pencil (edit) icon for the service to be modified.
    3. Modify any of the following fields:
        - Job Fee (enter a new numeric value)
        - Job Type (select a different option from the dropdown)
    4. Click the check (✔) icon to save the changes.

- **Expected Result**: The updated service details are saved and reflected immediately in the UI.
- **Postcondition**:  The freelancer's service record is updated in the database and reflected in their profile view.
- **Status**:
    - [ ] Pass  
    - [ ] Fail
