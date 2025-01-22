-- Question 1: Create an index on TotalAmount column in the bills table
CREATE INDEX IdxTotalAmount ON bills (TotalAmount);

-- Question 2: Drop an index named IdxEmail from the customer table
DROP INDEX IdxEmail ON customer;

-- Question 3: Create a user named bob with a password, restricted to localhost
CREATE USER 'bob'@'localhost' IDENTIFIED BY 'S$cu3r3!';

-- Question 4: Grant INSERT privilege to user bob on the bills database
GRANT INSERT ON bills.* TO 'bob'@'localhost';

-- Question 5: Change the password for user bob
ALTER USER 'bob'@'localhost' IDENTIFIED BY 'P$55!23';
