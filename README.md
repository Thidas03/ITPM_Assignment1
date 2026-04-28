# IT3040 – ITPM Assignment 1
## Transliteration Accuracy Testing

**Student ID:** IT23642478  
**Degree:** BSc (Hons) in Information Technology – Year 3  
**Semester:** Semester 1  
**Assignment:** Assignment 1 – Option 1 (For students familiar with Sinhala)

---

## 📌 Objective

This project evaluates the accuracy of the **Chat Sinhala transliteration** function available at:

👉 [https://www.pixelssuite.com/chat-translator](https://www.pixelssuite.com/chat-translator)

The goal is to identify **50 test cases where the system fails** to correctly convert chat-style Singlish input into Sinhala output, automate all identified scenarios using **Playwright**, and record the execution results in an Excel file.

---

---

## ⚙️ Prerequisites

- Python 3.11 or 3.12
- Google Chrome (recommended) or Playwright will use Chromium
- Git

---

## 🚀 Installation & Setup

### Step 1: Clone the repository
```bash
git clone https://github.com/Thidas03/ITPM_Assignment1.git
cd ITPM_Assignment1
```

### Step 2: Navigate to the test_automation folder
```bash
cd test_automation
```

### Step 3: Install required dependencies (one-time only)
```bash
pip install -U pip
pip install playwright openpyxl
python -m playwright install
```

---

## ▶️ How to Run the Tests

### Step 1: Go back to the root folder
```bash
cd ..
```

### Step 2: Run the Playwright script
```bash
python test_automation/test_automation.py --excel "test_automation/Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

### Step 3: Check the results
After the script finishes, open `Assignment 1 - Test cases.xlsx`. The **Actual output** and **Status** columns will be filled automatically.

---

## 📊 Test Case Details

## ✅ Singlish Input Types Covered

All **24 Singlish input types** specified in Appendix 1 are covered with at least 2 test cases each:

| # | Input Type | Test Cases |
|---|---|---|
| 1 | Question forms | Neg_003, Neg_034 |
| 2 | Command forms | Neg_004, Neg_005 |
| 3 | Greetings | Neg_001, Neg_012 |
| 4 | Requests | Neg_007, Neg_040 |
| 5 | Responses | Neg_008, Neg_040 |
| 6 | Repeated Words | Neg_009, Neg_036 |
| 7 | Inputs with Punctuation Marks | Neg_005, Neg_006 |
| 8 | Romanization / Spelling Variants | Neg_002, Neg_011, Neg_033, Neg_046 |
| 9 | Isolated English Word Insertions in Singlish | Neg_004, Neg_010, Neg_014, Neg_016 |
| 10 | Multi-Word English Phrases in Singlish | Neg_013, Neg_031, Neg_032 |
| 11 | English Digital Terms in Singlish | Neg_030, Neg_035, Neg_038 |
| 12 | Platform/App Names in Singlish | Neg_013, Neg_015 |
| 13 | English Abbreviations/Acronyms in Singlish | Neg_008, Neg_039 |
| 14 | English Clipped Forms in Singlish | Neg_043, Neg_044 |
| 15 | Place Names Embedded in Singlish | Neg_017, Neg_018 |
| 16 | Person Names Embedded in Singlish | Neg_019, Neg_020, Neg_037 |
| 17 | Inputs with Numbers and Numeric Suffixes | Neg_048, Neg_050 |
| 18 | Inputs with Currency | Neg_027, Neg_042 |
| 19 | Inputs with Time Formats | Neg_041, Neg_049, Neg_050 |
| 20 | Inputs with Dates | Neg_021, Neg_042 |
| 21 | Inputs with Unit of Measurements | Neg_026, Neg_045 |
| 22 | Inputs with Slang and Casual Phrasing | Neg_009, Neg_024, Neg_025, Neg_036, Neg_047 |
| 23 | Online Identifiers in Singlish | Neg_022, Neg_023 |
| 24 | Inputs Containing Emojis | Neg_009, Neg_016 |

---


