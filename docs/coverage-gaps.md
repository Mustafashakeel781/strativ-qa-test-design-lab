# Coverage Gaps

This document contains unclear or missing requirements identified during test design.

---

## 1. User Registration

### Coverage Gap 1

**Requirement:** Password must be at least 8 characters.

**Gap:** The maximum password length is not specified.

### Coverage Gap 2

**Requirement:** Email must be unique.

**Gap:** It is not specified whether email comparison is case-sensitive or case-insensitive.

**Example:**
- mustafa@gmail.com
- Mustafa@gmail.com

### Coverage Gap 3

**Requirement:** Password is required.

**Gap:** Allowed special characters are not mentioned.

**Examples:**
- @
- #
- $
- %

### Coverage Gap 4

**Requirement:** Registration is successful.

**Gap:** It is not specified whether email verification is required before login.

### Coverage Gap 5

**Requirement:** First Name and Last Name are required.

**Gap:** The maximum number of characters is not defined.

### Coverage Gap 6

**Requirement:** Email is required.

**Gap:** It is not mentioned whether leading or trailing spaces should be accepted or automatically trimmed.

---

## 2. Seat Requests

### Coverage Gap 1

**Requirement:** A user can request available seats.

**Gap:** It is not specified whether a user can cancel a previously submitted seat request.

### Coverage Gap 2

**Requirement:** The maximum allowed number of seats per user should be validated.

**Gap:** The exact maximum number of seats allowed per user is not specified.

### Coverage Gap 3

**Requirement:** A user should not submit the same request multiple times accidentally.

**Gap:** It is not specified how duplicate requests should be detected or prevented.

### Coverage Gap 4

**Requirement:** Seats should decrease after a successful request.

**Gap:** It is not specified what happens if two users request the last available seat at the same time.

### Coverage Gap 5

**Requirement:** The system should display a confirmation after a successful request.

**Gap:** The exact confirmation message and format are not specified.

### Coverage Gap 6

**Requirement:** A failed request should not decrease available seats.

**Gap:** The specific failure conditions such as network failure, timeout or server error are not defined.

---

## 3. AI Message Limits

### Coverage Gap 1

**Requirement:** Only logged-in users can send AI messages.

**Gap:** It is not specified what happens if the user's session expires while sending a message.

### Coverage Gap 2

**Requirement:** The user must have remaining message credits.

**Gap:** It is not specified how many message credits are provided each day.

### Coverage Gap 3

**Requirement:** The daily message limit should reset automatically.

**Gap:** It is not specified at what time the daily limit resets.

### Coverage Gap 4

**Requirement:** Messages longer than the allowed limit should not be accepted.

**Gap:** The maximum allowed message length is not specified.

### Coverage Gap 5

**Requirement:** The remaining message count should always be visible.

**Gap:** It is not specified where the remaining message count should be displayed.

### Coverage Gap 6

**Requirement:** Failed messages should not reduce message credits.

**Gap:** It is not specified which failure conditions such as network error, timeout or server error are included.

---

## 4. Image Upload

### Coverage Gap 1

**Requirement:** Only JPG, JPEG, and PNG files are allowed.

**Gap:** The maximum supported image dimensions are not specified.

### Coverage Gap 2

**Requirement:** The image size must not exceed the allowed limit.

**Gap:** The maximum allowed file size is not specified.

### Coverage Gap 3

**Requirement:** Duplicate image uploads should follow application rules.

**Gap:** It is not specified whether duplicate images should be allowed or rejected.

### Coverage Gap 4

**Requirement:** Uploaded image should be displayed.

**Gap:** It is not specified whether the image should appear immediately or after refreshing the page.

### Coverage Gap 5

**Requirement:** Upload process should display an error message if it fails.

**Gap:** The possible failure reasons such as network error, server error or storage issue are not defined.

### Coverage Gap 6

**Requirement:** Uploaded image should be stored successfully.

**Gap:** The storage location and storage behavior are not specified.

---

## 5. Task Status Transition

### Coverage Gap 1

**Requirement:** Only authorized users can change the task status.

**Gap:** The user roles and permissions are not specified.

### Coverage Gap 2

**Requirement:** A task can move through the defined workflow.

**Gap:** The complete list of allowed and restricted status transitions is not specified.

### Coverage Gap 3

**Requirement:** Completed tasks cannot be edited.

**Gap:** It is not specified whether completed tasks can be reopened by an Admin or Manager.

### Coverage Gap 4

**Requirement:** Task status history should be maintained.

**Gap:** It is not specified what information such as user, date, time or comments should be stored in the history.

### Coverage Gap 5

**Requirement:** A confirmation message should be displayed after a successful status update.

**Gap:** The exact confirmation message is not defined.

### Coverage Gap 6

**Requirement:** The updated task status should be visible immediately.

**Gap:** It is not specified whether the page refreshes automatically or updates dynamically.
