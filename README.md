# 🧠 Brute Force Attack Detection using Log Analysis (SOC Project)

## 📌 Objective
To simulate and detect brute force login attempts by analyzing Linux authentication logs.

---
## 🧰 Tools Used
- Kali Linux  
- Terminal  
- journalctl  

---
## 🧪 Steps Performed

### 1️⃣ Simulated Attack
- Performed multiple failed login attempts using su root  
- Entered incorrect password multiple times to simulate brute force pattern  

---
### 2️⃣ Log Collection
- Used system logs to monitor authentication activity  
- Command used:
bash - journalctl 

---
### 3️⃣ Log Filtering
- Filtered failed login attempts:
bash - journalctl | grep "authentication failure" 

---
### 4️⃣ Detection & Analysis
- Observed multiple failed login attempts within short time  
- Identified repeated targeting of root account  

---
### 5️⃣ Count Analysis
- Counted total failed attempts:
bash - journalctl | grep "authentication failure" | wc -l 

---
## 🔍 Findings
- Multiple authentication failures detected  
- Same user (root) targeted repeatedly  
- Attempts occurred within short time interval  

👉 Indicates a brute force attack pattern

---
## 📊 Result
Successfully simulated and detected brute force login attempts using log analysis techniques.

---
## 📸 Screenshots
- Failed login attempts (su root)  
- Authentication failure logs  
- Count of failed attempts  

---
## ⚠️ Note
This project was performed in a controlled lab environment for educational purposes.
