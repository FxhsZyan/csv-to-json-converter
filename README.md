# CSV to JSON Converter

A simple web app that uploads a CSV file and converts it into JSON, following a data map for field names, data types, and transformation rules.

## Live Demo

You can open the app here:

**https://bugtongzydme.dcism.org/**

## Features

- Upload a CSV file from your computer
- Convert the data to JSON with one click
- Preview the JSON output on the page
- Download the result as `output.json`

## Data Map

| Source Field (CSV) | Target Field (JSON) | Target Data Type | Transformation Rule                 |
| ------------------ | ------------------- | ---------------- | ----------------------------------- |
| student_id         | studentId           | Integer          | Convert string to integer           |
| first_name         | firstName           | String           | Capitalize first letter             |
| last_name          | lastName            | String           | Capitalize first letter             |
| course             | program             | String           | Convert to full program name        |
| year_level         | yearLevel           | Integer          | Convert string to integer           |
| email              | emailAddress        | String           | Convert to lowercase                |
| tuition_balance    | outstandingBalance  | Number           | Convert to decimal with 2 places    |

### Supported Course Codes

| Code | Program                                          |
| ---- | ------------------------------------------------ |
| BSIT | Bachelor of Science in Information Technology    |
| BSCS | Bachelor of Science in Computer Science          |
| BSIS | Bachelor of Science in Information Systems       |
| BSCE | Bachelor of Science in Computer Engineering      |
| BSEE | Bachelor of Science in Electrical Engineering    |
| BSME | Bachelor of Science in Mechanical Engineering    |
| BSBA | Bachelor of Science in Business Administration   |
| BSA  | Bachelor of Science in Accountancy               |
| BSN  | Bachelor of Science in Nursing                   |

Any course code not listed above is kept as it appears in the CSV.

## How to Use

1. Open the app at https://bugtongzydme.dcism.org/
2. Click **Choose File** and select a `.csv` file.
3. Click **Convert CSV to JSON**.
4. Review the output in the JSON Display section.
5. Click **Download JSON** to save the file.

### Expected CSV Columns

```
student_id,first_name,last_name,course,year_level,email,tuition_balance
```

## Running Locally

No installation is needed. Download `index.html` and open it in any modern web browser.

## Built With

- HTML
- CSS
- JavaScript (no external libraries)

## Author

**Zyann Bugtong**
IT 3206N, TTH 6:00 pm - 8:30 pm
