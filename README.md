Task-1: Joins Practice – SQL Code Description
This SQL script demonstrates the practical use of various SQL JOIN operations using two simple and relatable tables: patients and appointments. The purpose of this task is to understand how different types of joins work when retrieving data from multiple related tables. This is a fundamental concept in relational databases and essential for performing accurate data analysis.

The first table created is patients, which contains the basic details of patients. It includes two columns: patient_id (the primary key) and patient_name. The table is populated with sample data for four patients: Arjun, Sneha, Kabir, and Megha.

The second table is appointments, which records appointment details including appointment_id, patient_id, doctor_name, and appointment_date. Here, patient_id serves as a foreign key intended to relate to the patients table. The inserted data includes appointments for patient IDs 1, 2, and 5. Patient ID 5 is intentionally not present in the patients table to demonstrate how joins behave when the relationship is missing.

The script then includes four types of JOIN queries:

INNER JOIN
This join returns only the rows where there is a match between patients and appointments based on the patient_id. This means it will show only those patients who have an appointment record, excluding any patients without appointments and any appointments that do not have a corresponding patient.

LEFT JOIN
This join returns all rows from the patients table and the matched rows from the appointments table. If a patient does not have an appointment, the appointment-related columns will show NULL. This helps identify patients who are registered but haven’t booked any appointments yet.

RIGHT JOIN
This returns all rows from the appointments table and the matching records from the patients table. If an appointment exists without a valid patient (as in the case of patient_id = 5), it will still appear, and the patient fields will be NULL. This is useful to detect data integrity issues.

FULL OUTER JOIN
This join returns all records from both tables, whether a match exists or not. It helps to provide a complete picture of both tables. Since MySQL does not support FULL OUTER JOIN natively, an alternative using UNION of LEFT JOIN and RIGHT JOIN is included in the script. This workaround simulates full outer join behavior in MySQL environments.

The joins are tested with meaningful sample data that reflects real-world scenarios such as unmatched records and null handling. This makes it easier to understand how each type of join functions. Each query output highlights the differences between join types and shows how records are included or excluded based on the matching criteria.

This task serves as a strong foundation for understanding join operations in SQL. It is particularly useful for students, beginners, and database learners who are practicing SQL queries for projects or interviews. The code is clean, simple, and runs well in platforms like SQLFiddle, DB-Fiddle, or local SQL environments like MySQL Workbench and PostgreSQL.

In summary, this Task-1 script demonstrates INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN with meaningful examples, and prepares the learner for more complex multi-table queries in real database systems.


COMPANY:CODTECH IT SOLUTIONS
NAME:GNANA PREETHIKA A B
DURATION:4 WEEKS
MENTOR:NEELA SANTHOSH KUMAR

