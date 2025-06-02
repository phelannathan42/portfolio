#  Test Case: Spotify Login Page Functionality

## Objective
Ensure that the Spotify login page functions correctly across expected user behaviors, including valid and invalid login attempts.

---

## Test Case ID
TC-001-SPOTIFY-LOGIN

## Module
Authentication / Login

## Priority
High

---

## Pre-Conditions
- User is on the Spotify login page: https://accounts.spotify.com/en/login
- Test account credentials available:
  - Email: testuser@example.com
  - Password: TestPass123!

---

## Test Steps

| Step No | Action                                      | Expected Result                                         |
|---------|---------------------------------------------|---------------------------------------------------------|
| 1       | Navigate to the login page                  | Login form appears with email and password fields       |
| 2       | Enter valid email and password              | User is successfully logged in and redirected to homepage |
| 3       | Enter incorrect password                    | Error message appears: "Incorrect username or password."|
| 4       | Leave email blank and submit                | Error message prompts: "Please enter your email."       |
| 5       | Leave password blank and submit             | Error message prompts: "Please enter your password."    |
| 6       | Click “Forgot Password?” link               | Redirects to password recovery page                     |
| 7       | Try logging in with invalid email format    | Error: "Enter a valid email address"                    |

---

## Post-Conditions
- User is either logged in or remains on the login screen with appropriate error messages.

---

## Pass/Fail Criteria
- Test case is considered **Passed** if all expected results match actual behavior.
- **Failed** if any field behaves incorrectly or error messages are missing/inaccurate.

---

## Notes
- Test performed on Chrome (latest), Firefox, and Safari.
- Next step: Cross-browser testing + mobile view responsiveness.

