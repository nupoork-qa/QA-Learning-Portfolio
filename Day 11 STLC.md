# 🧪 Software Testing Documentation – STLC & Test Design

## 📌 Software Testing Life Cycle (STLC)
STLC defines the sequence of activities carried out during the testing process to ensure quality.

**Phases:**
1. Requirement Analysis  
2. Test Planning  
3. Test Case Development  
4. Test Environment Setup  
5. Test Execution  
6. Test Cycle Closure  

<img width="586" height="412" alt="image" src="https://github.com/user-attachments/assets/135b6e53-0ca8-49f8-823e-b126db86e84c" />

<img width="1051" height="493" alt="image" src="https://github.com/user-attachments/assets/a2aa7ef9-aaff-4627-a9a0-b2c8861d4968" />

---

## 📝 Test Plan Contents
A test plan defines the scope, approach, resources, and schedule of testing activities.

- Overview  
- Scope of testing  
- Features to be tested  
- Features not to be tested  
- Test Environments  
- Test Strategy  
- Defect Reporting Procedure  
- Roles & Responsibilities  
- Test Schedule  
- Test Deliverables  
- Entry & Exit Criteria  
- Suspension & Resumption Criteria  
- Tools  
- Risks & Mitigations  
- Approvals  

---

## 🔹 Use Case, Test Scenario & Test Case  

- **Use Case** → Describes the requirement.  
  - Actor: End user of the system  
  - Action: Steps performed  
  - Goal: Expected successful outcome  

- **Test Scenario** → High-level description of what to test (What).  

- **Test Case** → Step-by-step actions to validate functionality (How).  

---

### Example: E-commerce Purchase Flow  

**Use Case:** Buy a Product  
- **Actor:** Customer  
- **Goal:** Purchase a product successfully.  
- **Steps:**  
  1. Browse product catalog  
  2. Select a product and add to cart  
  3. Checkout  
  4. Enter shipping & payment details  
  5. Place order  
  6. Receive confirmation  

**Test Scenario:** Successful purchase with valid credit card.  

**Test Case – TC01: Purchase with valid credit card**  
- **Pre-condition:** User logged in, product in cart  
- **Steps:**  
  1. Enter valid shipping details  
  2. Enter valid card info (number, expiry, CVV)  
  3. Click "Place Order"  
- **Expected Result:**  
  - Order confirmed  
  - Payment processed  
  - Status updated  

**Additional Test Cases:**  
- TC02 – Invalid credit card number  
- TC03 – Insufficient funds  
- TC04 – Missing shipping address  
- TC05 – Guest checkout  

---

## 📊 Requirement Traceability Matrix (RTM)  

| Requirement ID | Requirement Description              | Test Case IDs  |
|----------------|--------------------------------------|----------------|
| REQ001         | User should be able to log in        | TC001, TC002   |
| REQ002         | System should display product details| TC003, TC004   |
| REQ003         | User can add items to shopping cart  | TC005, TC006   |

---

## ⚙️ Test Environment (Test Bed)  
- A dedicated platform for test execution  
- Includes required software, hardware, and network configs  
- Simulates production environment  

---

## ▶️ Test Execution  
**Activities:**  
- Execute test cases as per plan  
- Mark status (Passed/Failed/Blocked/Skipped)  
- Log defects for failed cases & assign bug IDs  
- Retest after bug fixes  
- Track defects until closure  

**Guidelines:**  
- Test execution happens in QA environment  
- Performed in multiple cycles  
- Includes manual & automation scripts  

---


