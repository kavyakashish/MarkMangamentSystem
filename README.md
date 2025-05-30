Mark Management System

Project Purpose:
To manage student examination marks, including adding, updating, deleting, and displaying student
marks, along with generating reports such as students with marks above a certain threshold, students scoring in a specific subject, and top scorers.



Database Structure:
CREATE TABLE StudentMarks (
StudentID INT PRIMARY KEY,
StudentName VARCHAR(100),
Subject VARCHAR(50),
Marks INT,
ExamDate DATE
);



Modules & Functionalities:

MarkAdd: Add new student marks

MarkUpdate: Update existing marks

MarkDelete: Remove student records

MarkDisplay: Show all records or search by StudentID

Reports:

Students with marks above a specified value

Students who scored in a specific subject

Top N students based on marks

Project Structure:

MarkWebApp/

├── WebContent/

│ ├── index.jsp

│ ├── markadd.jsp

│ ├── markupdate.jsp

│ ├── markdelete.jsp

│ ├── markdisplay.jsp

│ ├── reports.jsp

│ ├── report_form.jsp

│ └── report_result.jsp

├── src/

│ ├── com/

│ ├── dao/

│ │ └── MarkDAO.java

│ ├── model/

│ │ └── StudentMark.java

│ └── servlet/

│ ├── AddMarkServlet.java

│ ├── UpdateMarkServlet.java

│ ├── DeleteMarkServlet.java

│ ├── DisplayMarksServlet.java

│ ├── ReportServlet.java

│ └── ReportCriteriaServlet.java

└── WEB-INF/web.xml
