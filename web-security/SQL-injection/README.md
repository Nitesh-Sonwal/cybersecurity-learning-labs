# SQL Injection

## 1. Overview

- What is SQL Injection?
- SQL Injection (SQLi) is a web application vulnerability that occurs when an application improperly handles user input in SQL queries.

- How does it happen?
- An attacker may manipulate the SQL query to access, modify or delete database information without authorization.

## 2. Types of SQL Injection

- Error-based SQL Injection - 
Uses database error messages to reveal information about the database or query structure.
- UNION-based SQL Injection - 
Uses the SQL UNION operator to combine results from multiple queries and retrieve data from other database tables.
- Blind SQL Injection - 
Occurs when an application does not directly display database errors or query results. The attacker infers information from the application's responses.
- Time-based Blind SQL Injection - 
A type of blind SQL injection where database response delays are used to infer information

## 3. Practical Learning

**Platform:** PortSwigger Web Security Academy

**Topics Practiced:**
- SQL injection basics
- UNION SQL injection
- Error-based SQL injection
- Blind SQL injection(currently learning)

## 4. Tools Used

- Burp Suite - 
Used to intercept, modify and resend HTTP requests during web application security testing.
- Chrome Developer Tools - 
Used to intercept HTTP requests and responses, query parameters, headers and browser storage through the Network and Application panels.

## 5. Learning Progress

Currently practicing SQL Injection vulnerabilities through controlled labs to understand how user input affects database queries and how vulnerabilities can be identified using Burp Suite.


## 6. Key Learnings

- SQL Injection occurs when user input is improperly handled in SQL queries.

- Error messages can reveal information about database queries.

- Blind SQL Injection requires observation skills and deduction of responses for inferring information from application behavior.

- HTTP requests and responses help understand how user input reaches a web application.

- Burp Suite can be used to inspect and manipulate HTTP requests during security testing.

## 7. Prevention

- Parameterized Queries: Separate SQL code from user-supplied data.

- Prepared Statements: Use prepared statements to prevent input from changing query structure.

- Input Validation: Validate input according to expected data types and formats.

- Least Privilege: Give database accounts only the permissions they require.

- Safe Error Handling: Avoid exposing sensitive database details in error message

## 8. References

- [PortSwigger Web Security Academy - SQL Injection](https://portswigger.net/web-security/sql-injection)
- [OWASP - SQL Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)