# Course 4: Tools of the Trade – Linux & SQL

---

## 📘 Module 1: Operating Systems & Virtualization

### Key Concepts
- Operating systems connect hardware and applications  
- Common OS: Windows, Linux, macOS  
- Legacy operating systems are outdated and vulnerable  

---

### Virtualization
- Virtual Machines (VMs) simulate real systems  
- Used for:
  - Malware testing  
  - Isolated environments  
- Important in cybersecurity  

---

### Key Learning
- Keeping systems updated reduces vulnerabilities  
- Legacy systems increase security risks  
- Virtualization helps in safe testing environments  

---

## 📘 Module 2: Linux Fundamentals

### Linux Architecture
- User → Applications → Shell → Kernel → Hardware  

---

### Key Components
- Kernel → manages processes  
- Shell → command-line interface  
- File system → organizes data  

---

### Package Management
- APT (Debian-based)  
- YUM / RPM (Red Hat-based)  

---

### Key Learning
- Linux is widely used in cybersecurity  
- Understanding Linux fundamentals is essential  
- Package management helps maintain system security  

---

## 📘 Module 3: Linux Commands & File System

### File System Structure
- `/` → root directory  
- `/home` → user files  
- `/etc` → configuration files  
- `/tmp` → temporary files (security risk)  

---

### Linux Commands (SOC Focus)

```bash
pwd    # current directory
ls     # list files
cd     # change directory
cat    # view file content
head   # first lines
tail   # last lines

mkdir  # create directory
rmdir  # remove directory
rm     # delete files
cp     # copy files
mv     # move/rename files
touch  # create file

grep   # search text patterns
find   # search files
sort   # sort output
uniq   # remove duplicates
wc     # word/line count

ls -l  # view permissions
chmod  # change permissions
```

---

### Key Concepts
- File management helps handle system data  
- Search & filtering are critical for investigations  
- Permissions follow the Principle of Least Privilege  

---

### Key Learning
- Linux CLI is essential for SOC investigations  
- Logs and files are primary data sources  
- Permissions control secure access  

---

## 📘 Module 4: Databases & SQL

### What is SQL?

SQL (Structured Query Language) is used to store, retrieve, and analyze structured data in databases.  
Security analysts use SQL to investigate logs, user activity, and suspicious behavior.

---

### SQL Concepts & Usage

```sql
-- Basic query
SELECT column_name FROM table;

-- Filtering data
SELECT * FROM users
WHERE name = 'Saksham';

-- Operators
-- =, <, >, <=, >=, !=, BETWEEN

-- Pattern matching
SELECT * FROM users
WHERE name LIKE 'a%';

-- Sorting results
SELECT * FROM users
ORDER BY column_name;

-- Limit results
SELECT * FROM users
LIMIT 5 OFFSET 10;

-- Join example (very important in SOC work)
SELECT users.name, logs.event
FROM users
INNER JOIN logs
ON users.id = logs.user_id;

-- Aggregate functions
SELECT COUNT(*) FROM users;
SELECT AVG(age) FROM users;
SELECT SUM(amount) FROM transactions;
```

---

### Key Concepts
- SQL filtering helps narrow down relevant data  
- Pattern matching helps detect suspicious entries  
- Joins help correlate multiple data sources  
- Aggregate functions help in analysis and reporting  

---

### SQL vs Linux
- Linux → works on logs and files  
- SQL → works on structured databases  
- Both are used together in real SOC investigations  

---

### Key Learning
- SQL is essential for analyzing structured data  
- Helps investigate user activity and logs  
- Useful in identifying suspicious behavior  
- Key skill for SOC analysts  

---

## 🎯 My Key Learning

- Linux is essential for SOC investigations  
- Command-line skills are critical  
- File permissions secure systems  
- SQL helps analyze large datasets efficiently  
- Practical skills matter more than theory in cybersecurity  
