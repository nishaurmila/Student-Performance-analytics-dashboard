# Student-Performance-analytics-dashboard:-
Interactive student performance analytics dashboard with CSV import and grade prediction

1. Project Type
A web-based analytics system that:

>>Displays student academic performance
>>Analyzes attendance and marks
>>Identifies at-risk students
>>Generates performance insights
>>Predicts student grades
>>Imports and exports CSV data
>>Visualizes data using interactive charts

2. Technology Stack
Component	Technology:-

Frontend	HTML5
Styling	CSS3
Programming Logic	JavaScript (Vanilla JS)
Charts	Chart.js v4.4.1
Data Storage	In-Memory JavaScript Objects
File Processing	FileReader API
Data Import	CSV Upload
Data Export	CSV Generation
Hosting	Static Website

3. Languages Used
>>HTML
(Purpose):
Website structure
Dashboard layout
Cards
Tables
Forms
Navigation
>>CSS
(Purpose):
Dark Theme UI
Responsive Layout
Cards
Dashboard Styling
Animations
Color System
Features Found:
CSS Variables
:root{
--bg:#0F1117;
--purple:#7C6FF7;
}
Grid Layout
Flexbox
Hover Effects
Fade Animations
Responsive Design

>>JavaScript
(Purpose):
Business Logic
Data Processing
Student Analytics
Chart Rendering
CSV Handling
Predictions
Functions found:
generateStudents()
parseCSV()
buildDashboard()
buildSubjects()
buildAtRisk()
showPage()
4. Visualization Library
Chart.js
(Loaded from CDN):
https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js

>>Purpose:
Interactive charts
Subject analysis
Performance comparison
Attendance tracking

>>Visualization Types:-
1.Bar Charts
Used for:
~Subject-wise scores
~Student comparison
Example:
Math      ████████
Science   ██████
English   ███████

2.Pie Charts
Used for:
~Grade Distribution
~Pass vs Fail
Example:
A Grade 40%
B Grade 30%
C Grade 20%

3.Doughnut Charts
Used for:
~Attendance Categories
~Performance Categories

4.Line Charts
Used for:
~Trend Analysis
~Performance Growth

5. Data Source
>>Generated Data:-
our website creates demo data using:
</> JavaScript
generateStudents(60)
This generates:
~Student Names
~IDs
~Attendance
~Marks
~Grades
~Percentages

>>CSV Data Import
Uses:
</> JavaScript
FileReader()
Purpose:
~Read uploaded CSV file
~Convert CSV to JavaScript objects
~Populate dashboard

*Workflow*:-
Upload CSV
      ↓
FileReader
      ↓
parseCSV()
      ↓
Store in JS Array
      ↓
Dashboard Refresh
6. Database Analysis:-
Our project currently stores data in:
</> JavaScript
let students = []
>>This means:
~Data exists only while page is open

>>Recommended Database
SQLite
~Small
~Fast
~Easy

>>Intermediate
MySQL
Tables:
</> SQL
~Students
~Subjects
~Attendance
~Results

7. Connectivity Architecture
(Current Architecture):-
Browser
   ↓
HTML
CSS
JavaScript
   ↓
Chart.js

(Future Architecture):-
Frontend
   ↓
REST API
   ↓
Backend (Flask/Django)
   ↓
MySQL/MongoDB

8. Analytics Features
>>Student Performance Analysis
Calculates:
~Total Marks
~Percentage
~Grade
~Rank
>>Attendance Analysis
Tracks:
Attendance %
~Low Attendance
~High Attendance

>>Risk Detection
~Function detected:
</> JavaScript
getRisk()

~Categories:
</> JavaScript
Low Attendance

Attendance < 75%
Low Score
Percentage < 40%

Both
Low Attendance + Low Score

9. Machine Learning Module
>>Page found:
ML Predict

>>Purpose:
Predict Grade
Predict Score
Estimate Performance
It appears to be rule-based prediction using JavaScript calculations.

10. CSV Processing Module
Features detected:
Upload CSV
</> JavaScript
openImport()

Read CSV
</> JavaScript
FileReader()

Parse CSV
</> JavaScript
parseCSV()

Export CSV
</> JavaScript
exportCSV()

(Workflow):-

Upload CSV
      ↓
Read File
      ↓
Parse Data
      ↓
Dashboard
      ↓
Analytics
      ↓
Export Results

11. Dashboard Modules
Your project contains these sections:

Dashboard:-
Overall Statistics

Students:-
Student List

Subjects:-
Subject-wise Analysis

At Risk:-
Weak Students Detection

ML Predict:-
Prediction System

12. UI/UX Features
Dark Theme
</> CSS
#0F1117
Professional dashboard appearance.

Responsive Design:-
**Works on:
~Desktop
~Laptop
~Tablet
~Mobile

Interactive Navigation:-
</> JavaScript
showPage()
Switches dashboard sections without reloading.

Toast Notifications:-
Function:
</> JavaScript
showToast()

Used for:
~Success messages
~Upload confirmation
~Errors

