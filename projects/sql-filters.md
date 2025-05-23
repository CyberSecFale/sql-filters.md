# sql-filters.md

# SQL Filters for Security Queries

I applied filters to SQL queries to identify potential security issues in a database. Using `WHERE` clauses, I filtered logs to find unauthorized access attempts, such as repeated failed login attempts from a single IP.

**Example Query:** `SELECT * FROM login_logs WHERE status = 'failed' AND ip_address = '192.168.1.100';`  
**Outcome:** Identified and flagged suspicious activity for further investigation.
