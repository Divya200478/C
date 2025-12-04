STUDY TRACKER APPLICATION

---------------------------------------------------


Author : Divya Santosh date 
Date Created : 28/07/2025
Language : Java
File Output : Study.csv (for exported logs)

DESCRIPTION

----------------------------------------------------

Study Tracker is a Java-based console application designed to help students keep a log of their daily study activities. The system allows users to:

Record study logs with subject, duration, and description.
Display all recorded logs.
Summarize logs based on date or subject.
Export logs into a CSV file for future use or sharing.

FEATURES

--------------------------------------------------

Insert New Log
Records today's date automatically.
Prompts for subject name, duration (in hours), and a brief description.
Display All Logs

Lists all study entries in the format:
YYYY-MM-DD | Subject | Duration | Description
Summary by Date

Aggregates and displays total study hours per day.
Summary by Subject

Aggregates and displays total study hours per subject.
Export to CSV

Exports all records to a file named Study.csv in the following format:
Date,Subject,Duration,Description
Exit

Cleanly terminates the application.

REQUIREMENTS

----------------------------------

Java Development Kit (JDK) 8 or above.
A terminal or IDE that supports console input/output.

TECHNOLOGIES USED

-----------------------------------

Language: Java Packages & APIs: java.util.* → Data structures (ArrayList, TreeMap), user input via Scanner. java.time.LocalDate → Auto-captures the current date for study logs. java.io.* → File handling and CSV export.

PROJECT FLOW

-----------------------------------------
Launch the application → Main Menu displayed
Choice 1: Insert new study log → User provides subject, duration, description → Date auto-generated.
Choice 2: Display all study logs stored in memory.
Choice 3: Display summary grouped by date (total hours per date).
Choice 4: Display summary grouped by subject (total hours per subject).
Choice 5: Export all study logs to MarvellousStudy.csv.
Choice 6: Exit application.

CLASSES AND RESPONSIBILITIES

----------------------------------------------------------------------------------------

StudyLog

Represents a single study session. Attributes: LocalDate date, String subject, double duration, String description. Methods: Constructor, getters, toString().

StudyTracker

Manages all logs in memory. Acts as a controller for StudyLog database. Methods: InsertLog(), DisplayLog(), SummaryByDate(), SummaryBySubject(), ExportCSV().

StudyTrackerApp (Main Class)

Contains main() method. Handles menu-driven interface and user input. Calls appropriate methods from StudyTracker.

EXAMPLE USAGE (CONSOLE FLOW)

------------------------------------------------------------------

===== Marvellous Study Tracker =====

Insert Study Log
Display All Logs
Summary by Date
Summary by Subject
Export to CSV
Exit Enter choice: 1
Enter Subject: Java Programming Enter Duration (Hours): 2.5 Enter Description: Practiced ArraysList and TreeMap Study log added successfully! (for date: 2025-09-13) Sample Exported CSV (MarvellousStudy.csv)

Date, Subject, Duration, Description 2025-09-13, Java Programming, 2.5, Practiced ArraysList and TreeMap 2025-09-13, Database, 1.5, Solved SQL Joins




