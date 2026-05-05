# 📘 Test Cases – Shopping List Mobile App

## 🎯 Objective
Validate the behavior of the item creation feature, focusing on input handling, validation rules, and system responses.

---

## 🧪 Test Cases

### ✅ TC01 – Valid Item Creation
**Description:** Validate successful item creation with valid inputs  

**Steps:**
1. Enter a valid item name  
2. Enter a valid quantity (e.g., 1)  
3. Tap the add button  

**Expected Result:**
- Item is successfully added to the list  

---

### ⚠️ TC02 – Empty Fields
**Description:** Validate system behavior when required fields are empty  

**Steps:**
1. Leave the “New Item” field empty  
2. Leave the “Quantity” field empty  
3. Tap the add button  

**Expected Result:**
- System prevents submission  
- Validation message is displayed **or** button is clearly disabled  

---

### ❌ TC03 – Invalid Quantity (Text Input)
**Description:** Validate that the quantity field rejects non-numeric values  

**Steps:**
1. Enter a valid item name  
2. Enter text in the quantity field (e.g., "abc")  
3. Tap the add button  

**Expected Result:**
- System rejects non-numeric input  
- Validation message is displayed  

---

### 🔢 TC04 – Decimal Quantity
**Description:** Validate behavior when decimal values are entered  

**Steps:**
1. Enter a valid item name  
2. Enter a decimal value (e.g., 0.5 or 1.5)  
3. Tap the add button  

**Expected Result:**
- System accepts or properly validates decimal values  

---

### 📏 TC05 – Long Item Name
**Description:** Validate system behavior with long text input  

**Steps:**
1. Enter a very long text in the “New Item” field  
2. Tap the add button  

**Expected Result:**
- System enforces maximum length **or** handles input without breaking  

---

### 📊 TC06 – Long Quantity Input
**Description:** Validate behavior with large numeric input  

**Steps:**
1. Enter a valid item name  
2. Enter a very large numeric value in “Quantity”  
3. Tap the add button  

**Expected Result:**
- System validates or limits input size appropriately  

---

## 📌 Notes
- Test cases were executed using a real device environment via BrowserStack  
- Observed results and issues are documented in the `bug-reports` section  
- Evidence for each test case is available in the `/evidence` folder  
