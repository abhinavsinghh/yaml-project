# Python YAML Student Info Application

This project is a simple Python application that reads student data from a YAML file and allows users to display all students and filter them based on GPA.

## Features
- Reads student data from a YAML file.
- Displays all student details.
- Filters students based on a minimum GPA entered by the user.

## Prerequisites
Ensure you have Python 3 installed. You can check by running:

\`\`\`bash
python3 --version
\`\`\`

## Installation
### 1. Install Dependencies
Since modern Ubuntu systems use an externally managed environment, install \`PyYAML\` in a virtual environment:

\`\`\`bash
# Create a virtual environment
python3 -m venv venv

# Activate the virtual environment
source venv/bin/activate

# Install dependencies
pip install pyyaml
\`\`\`

Alternatively, you can install it globally (not recommended):

\`\`\`bash
pip install --break-system-packages pyyaml
\`\`\`

### 2. Create the \`students.yaml\` File
Create a file named \`students.yaml\` in the same directory as your script and add:

\`\`\`yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
  - name: Charlie
    age: 20
    major: Physics
    gpa: 3.9
  - name: David
    age: 23
    major: Chemistry
    gpa: 3.2
  - name: Eva
    age: 21
    major: Computer Science
    gpa: 3.7
\`\`\`

### 3. Run the Application
Ensure both \`app.py\` and \`students.yaml\` are in the same directory. Then, run:

\`\`\`bash
python3 app.py
\`\`\`

## Expected Output
\`\`\`
All Students:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Bob, Age: 22, Major: Mathematics, GPA: 3.5
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: David, Age: 23, Major: Chemistry, GPA: 3.2
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7

Enter minimum GPA to filter students: 3.6

Students with GPA >= 3.6:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7
\`\`\`


## Future Enhancements
- Sort students by GPA.
- Add functionality to update student records.
- Save filtered results to a new YAML file.

## License
This project is open-source and free to use.

---

