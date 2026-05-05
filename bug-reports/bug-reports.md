# 📘 Bug Reports – Shopping List Mobile App

## 🎯 Objective
Document issues identified during test execution, including input validation problems and user experience gaps.

---

## 🐞 Reported Bugs

### ⚠️ BUG-01 – No Feedback on Invalid Input
**Severity:** Medium  
**Priority:** High  

**Description:**  
The add button does not provide feedback when required fields are empty or invalid.

**Steps to Reproduce:**
1. Leave the “New Item” field empty  
2. Leave the “Quantity” field empty or invalid  
3. Tap the add button  

**Expected Result:**
- Button should be disabled **or**  
- Validation message should be displayed  

**Actual Result:**
- No action is performed  
- No visual feedback or error message is shown  

**Impact:**
- Poor user experience  
- User may not understand why the action failed  

---

### ❌ BUG-02 – Quantity Field Accepts Non-Numeric Input
**Severity:** High  
**Priority:** High  

**Description:**  
The quantity field allows text input (e.g., "abc"), which leads to invalid data being added.

**Steps to Reproduce:**
1. Enter a valid item name  
2. Enter text in the “Quantity” field (e.g., "abc")  
3. Tap the add button  

**Expected Result:**
- Only numeric values should be accepted  
- Validation message should be displayed  

**Actual Result:**
- Text input is accepted  
- Item is added with invalid quantity  

**Impact:**
- Data inconsistency  
- Potential downstream issues  

---

### 📏 BUG-03 – No Input Length Validation
**Severity:** Medium  
**Priority:** Medium  

**Description:**  
Both “New Item” and “Quantity” fields accept excessively long inputs without restriction.

**Steps to Reproduce:**
1. Enter a very long text in the “New Item” field  
2. Enter a very large number in the “Quantity” field  
3. Tap the add button  

**Expected Result:**
- System should enforce maximum length  
- Input should be limited or validated  

**Actual Result:**
- Inputs are accepted without restriction  

**Impact:**
- Potential UI issues  
- Risk of performance or data handling problems  

---

## 📌 Notes
- Bugs were identified during exploratory and functional testing  
- Tests executed on a real device environment using BrowserStack  
- Supporting evidence is available in the `/evidence` folder  
