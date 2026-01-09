# new-user-registration-User-Story
This repository documents the user story, wireframe/UI requirements, and workflow for the ‘New User Registration’ feature, enabling users to self-register and create login credentials online.

# New User Registration – Project Documentation

## 📌 Project Overview
This project documents the **user story, wireframe/UI requirements, and workflow** for the **New User Registration** feature on [http://mywebsite.com](http://mywebsite.com).  
The feature allows new users to self-register and create login credentials online without waiting for credentials via paper mail.

---

## 📖 User Story

**As a:** New user of [http://mywebsite.com](http://mywebsite.com)  
**I want to:** Be able to register online  
**So that:** I can create my login credentials myself without waiting to receive them via paper mail

### Acceptance Criteria
1. System displays a **‘Register’** hyperlink adjacent to the left of the **‘Login’** hyperlink.  
2. On click of **‘Register’**, the system navigates the user to the **New User Registration** page in the same browser window.  
3. System allows the user to enter registration data.  
4. On click of **Register** command button, system performs validations:  
   - All required data is entered  
   - Email address is in a valid format  
   - Email address is unique  
   - Password entered is in a valid format  
   - Re-entered password matches the password entered  
   4.1 If all validations pass → navigate user to **Registration Complete** page  
   4.2 If validations fail → display inline error messages  
5. On click of **Cancel** button → discard entered data and navigate user to the home page.

---

## 🖼 Wireframe & UI Requirements

### Registration Link
| ID | Field Name | Field Type | Content | Required Field? | Notes |
|----|------------|------------|---------|----------------|-------|
| 1  | Register   | Hyperlink  | N/A     | No             | On click, navigate to **New User Registration** page |

### New User Registration Page
| ID | Field Name | Field Type | Content | Required Field? | Notes |
|----|------------|------------|---------|----------------|-------|
| 1  | New User Registration | Text | N/A | No | Page title |
| 2  | * are required fields | Text | N/A | No |  |
| 3  | Email Address | Text Box | Alpha Numeric with special characters | Yes | Min: 6, Max: 100 |
| 4  | Password | Text Box | Alpha Numeric | Yes | Encrypted, Min: 8, Max: 16 |
| 5  | Re-enter Password | Text Box | Alpha Numeric | Yes | Encrypted, Min: 8, Max: 16 |
| 6  | Gender | Radio Button | Male, Female | No | No default selection |
| 7  | Security Question | Dropdown | Predefined questions | Yes | Alphabetical order, no default selection |
| 8  | Security Answer | Text Box | Alpha Numeric | Yes | Min: 2, Max: 36 |
| 9  | Register | Command Button | N/A | N/A | If validations pass → navigate to **Registration Complete**, else show errors |
| 10 | Cancel | Command Button | N/A | N/A | Discard data, navigate to home page |

### Registration Complete Page
| ID | Field Name | Field Type | Content | Required Field? | Notes |
|----|------------|------------|---------|----------------|-------|
| 1  | Registration Complete | Text | N/A | No | Page title |
| 2  | Congratulations message | Text | N/A | No |  |
| 3  | Please Login to manage your account | Hyperlink | N/A | No | Navigate to **Login** page |

---

## ⚠️ Inline Error Messages

| Failed Validation | Error Message |
|------------------|---------------|
| Required data missing | `<Field Name>` is a required data. |
| Email format invalid | Please enter a valid email address. |
| Email not unique | Email address entered is already associated with an active account |
| Password invalid | Password must be between 8 and 16 characters |
| Re-entered password mismatch | Re-entered password does not match the password entered |

---

## 🔄 Workflow
1. User clicks **Register** hyperlink from homepage.  
2. System navigates to **New User Registration** page.  
3. User fills in registration fields.  
4. User clicks **Register** button → system performs validations:  
   - Success → navigate to **Registration Complete** page  
   - Failure → display inline errors  
5. User clicks **Cancel** → system discards data and navigates back to homepage.

   ---

---
rtfolio artifact** for **MIS, Business Analyst, or Software Engineering projects**.
