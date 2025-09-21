# Software Testing Terminology

## Regression Testing
Regression testing is the process of testing a software application to ensure that new changes (like updates, bug fixes, or new features) do not negatively impact the existing functionality of the software.  

**Example:**  
Imagine you have a mobile app that allows users to log in, view their profile, and send messages. If a developer adds a new feature, such as uploading profile pictures, regression testing ensures that after this change, users can still log in, view their profiles, and send messages without issues.

### Types of Regression Testing
- **Unit Regression Testing**: Test only the specific changes made by the developer.  
- **Regional Regression Testing**: Test the changed part along with connected modules.  
  - *Impact Analysis Meeting* is conducted to figure out affected parts (involving testing & development teams).  
- **Full Regression Testing**: Test both the changed part and the rest of the software to be thorough.  
  - Example: If changes are made across multiple areas, test everything in one full round.

---

## Re-Testing
When a developer fixes a bug, testers re-check the bug fix.  

- If fixed → Tester closes the bug.  
- If not fixed → Tester reopens the bug and assigns it back to the developer.  

**Example:**  
- Build 1.0 released → Test team found defects (IDs: 1.0.1, 1.0.2).  
- Build 1.1 released → Retesting focuses on verifying those specific defects.  

---

## Re-Testing vs Regression Testing
- **Re-Testing**: Specifically checks if a fixed bug is resolved.  
- **Regression Testing**: Ensures fixes or changes don’t break existing functionality in other modules.  

**Example:**  
- Modules: Admin, Purchase, Finance.  
- Bug found in Purchase → Retest Purchase bug.  
- Regression test Finance → because it depends on Purchase.

---



## Exploratory Testing
- Explore the application without detailed requirements.  
- Identify scenarios and document them for testing.  

**Drawbacks:**  
- May mistake bugs for features (or vice versa).  
- Time-consuming.  
- Hidden bugs may go unnoticed.  

---

## Adhoc Testing
- Informal, unplanned testing.  
- No documentation or test cases.  
- Tester must have some knowledge of the app.  

---

## Monkey Testing
- Random, unplanned testing without knowledge of the app.  
- Often used for gaming applications.  

---

## Exploratory vs Adhoc vs Monkey Testing
| Testing Type | Documentation | Knowledge | Purpose |
|--------------|--------------|-----------|---------|
| **Exploratory** | None | Low | Learn/explore functionality |
| **Adhoc** | None | Some | Break system / find corner bugs |
| **Monkey** | None | None | Random break test (games) |

---

## Positive Testing
Ensures system behaves correctly with **valid inputs**.  

**Examples:**  
- Valid login credentials → user logs in.  
- Calculator → correct sum for valid numbers.  
- Form submission → successful with valid data.  

---

## Negative Testing
Ensures system handles **invalid inputs** gracefully.  

**Examples:**  
- Wrong login password → rejected.  
- Upload invalid file format → handled properly.  
- Expired credit card → flagged during payment.  

---

## End-to-End Testing
Tests the **entire application flow** from start to finish.  

**Example (E-commerce App):**  
1. User logs in.  
2. Adds items to cart.  
3. Proceeds to checkout.  
4. Payment processed, confirmation generated.  
5. Email confirmation received.  

Checks across **UI + API + DB** integration.

---

## Globalization & Localization Testing
- **Globalization Testing**: Ensures the app works across regions, languages, currencies, date formats.  
- **Localization Testing**: Ensures app is adapted for a specific locale (translations, cultural preferences, region-specific rules).  

**In short:**  
- Globalization → Works **anywhere** in the world.  
- Localization → Works **well** in one specific region.  

