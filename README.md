Table Descriptions:
batch

bat_id: Integer, primary key. Unique identifier for each batch.
bat_name: Variable character string (up to 30 characters). Name of the batch.
domain

dom_id: Integer, primary key. Unique identifier for each domain.
dom_name: Variable character string (up to 30 characters). Name of the domain.
professional

prof_id: Integer, primary key. Unique identifier for each professional.
prof_name: Variable character string (up to 30 characters). Name of the professional.
salary

sal_id: Integer, primary key. Unique identifier for each salary record.
fee

fee_id: Integer, primary key. Unique identifier for each fee record.
mentor

men_id: Integer, primary key. Unique identifier for each mentor.
men_name: Variable character string (up to 50 characters). Name of the mentor.
men_email: Variable character string (up to 50 characters). Email of the mentor.
bat_id: Integer, foreign key. References batch(bat_id).
prof_id: Integer, foreign key. References professional(prof_id).
sal_id: Integer, foreign key. References salary(sal_id).
learners

len_id: Integer, primary key. Unique identifier for each learner.
len_name: Variable character string (up to 50 characters). Name of the learner.
len_email: Variable character string (up to 50 characters). Email of the learner.
bat_id: Integer, foreign key. References batch(bat_id).
dom_id: Integer, foreign key. References domain(dom_id).
fee_id: Integer, foreign key. References fee(fee_id).
DESC Command:
The DESC (or DESCRIBE) command in SQL is used to display the structure of a table. It provides information about the columns in the table, including:

Field: The name of the column.
Type: The data type of the column.
Null: Whether the column can contain NULL values.
Key: If the column is part of a primary key (PRI), foreign key (MUL), or unique key (UNI).
Default: The default value of the column.
Extra: Additional information about the column (e.g., if it is auto-increment).
When you run DESC table_name;, it outputs the schema of the specified table.
