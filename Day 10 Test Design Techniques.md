#  Test Design Techniques

**Test Design Techniques** help testers design better test cases while reducing the number of cases to be executed.

### Main Techniques
1. Equivalence Class Partitioning (ECP)  
2. Boundary Value Analysis (BVA)  
3. Decision Table Testing  
4. State Transition Testing  
5. Error Guessing  

---

## 1. Equivalence Class Partitioning (ECP)
Partition input data into **valid** and **invalid** classes.  
This reduces redundant test cases and saves time.  

**Example:** Field: *Name* (Only alphabets allowed)  

| Equivalence Class     | Valid/Invalid | Test Data |
|------------------------|---------------|-----------|
| A–Z                   | Valid         | XYZ       |
| a–z                   | Valid         | zyz       |
| Special Characters    | Invalid       | @#$%      |
| Spaces                | Invalid       | Xy z      |
| Numbers               | Invalid       | 1234      |

---

## 2. Boundary Value Analysis (BVA)
Focus on testing the **boundaries** of valid/invalid input values.  

**Example:** Field: *Age* (Allowed: 18–35)  

| Parameter | Value | Valid/Invalid |
|-----------|-------|---------------|
| Min       | 18    | Valid         |
| Min–1     | 17    | Invalid       |
| Min+1     | 19    | Valid         |
| Max       | 35    | Valid         |
| Max–1     | 34    | Valid         |
| Max+1     | 36    | Invalid       |

---

## 3. Decision Table Testing
- Also called **Cause–Effect Table**.  
- Useful when there are **multiple conditions** and **corresponding actions**.  
- Helps in identifying test cases based on input combinations.  

---

## 4. State Transition Testing
Application changes **state** based on different inputs.  
Tester provides both **positive** and **negative** inputs to verify behavior.  

**Example:** Login Page – Account locks after 3 failed attempts.  

| State        | Input Condition    | Next State  |
|--------------|--------------------|-------------|
| S1 (1st try) | Correct Password   | S4 (Home)   |
| S1 (1st try) | Incorrect Password | S2 (2nd try)|
| S2 (2nd try) | Correct Password   | S4 (Home)   |
| S2 (2nd try) | Incorrect Password | S3 (3rd try)|
| S3 (3rd try) | Correct Password   | S4 (Home)   |
| S3 (3rd try) | Incorrect Password | S5 (Locked) |
| S5           | –                  | "Account locked. Contact Admin" |

---

## 5. Error Guessing
Error guessing is based on **tester’s experience and intuition**.  
The tester identifies areas where bugs are **likely to occur**.  

**Common Examples:**
- Leaving required fields empty  
- Uploading unsupported file formats  
- Entering special characters in numeric fields  
