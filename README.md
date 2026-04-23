#              ✨             Basic Linux Commands

<p align="center">
  <i>Includes Question, Explanation, Syntax & Example</i>
</p>

---

## 📁 1. Create Directory & Subdirectory, then Remove Subdirectory

### ❓ Question

Create a directory and a subdirectory, then remove the subdirectory.

### 💡 Explanation

Use `mkdir` to create directories and `rmdir` (empty) or `rm -r` (non-empty) to remove.

### ⚙️ Syntax

```bash id="a1"
mkdir directory_name
mkdir parent/subdirectory
rmdir subdirectory
rm -r subdirectory
```

### 🧪 Example

```bash id="a2"
mkdir mainDir
mkdir mainDir/subDir
rmdir mainDir/subDir
```

---

## 🔍 2. Search a Word in a File

### ❓ Question

Search a word in a file and display matching lines.

### 💡 Explanation

Use `grep` to find matching lines.

### ⚙️ Syntax

```bash id="b1"
grep "word" filename
```

### 🧪 Example

```bash id="b2"
grep "hello" file.txt
```

---

## 🔐 3. Change File Permissions

### ❓ Question

Change file permissions.

### 💡 Explanation

Use `chmod` to modify permissions.

### ⚙️ Syntax

```bash id="c1"
chmod permissions filename
```

### 🧪 Example

```bash id="c2"
chmod 755 file.txt
```

---

## 🌐 4. Display IP Address

### ❓ Question

Display IP address of the system.

### 💡 Explanation

Use `ip addr` or `ifconfig`.

### ⚙️ Syntax

```bash id="d1"
ip addr
```

### 🧪 Example

```bash id="d2"
ip addr show
```

---

## 👤 5. Create New User & Set Password

### ❓ Question

Create a new user and assign a password.

### 💡 Explanation

Use `useradd` and `passwd`.

### ⚙️ Syntax

```bash id="e1"
sudo useradd username
sudo passwd username
```

### 🧪 Example

```bash id="e2"
sudo useradd john
sudo passwd john
```

---

## 🧠 6. Display CPU Information

### ❓ Question

Display CPU information.

### 💡 Explanation

Use `lscpu`.

### ⚙️ Syntax

```bash id="f1"
lscpu
```

### 🧪 Example

```bash id="f2"
lscpu
```

---

## 🌎 7. Find IP of Website

### ❓ Question

Find IP address of a website.

### 💡 Explanation

Use `nslookup` or `ping`.

### ⚙️ Syntax

```bash id="g1"
nslookup domain
```

### 🧪 Example

```bash id="g2"
nslookup google.com
```

---

## 🔑 8. SSH Connection

### ❓ Question

Attempt SSH connection.

### 💡 Explanation

Use `ssh` to connect to a remote system.

### ⚙️ Syntax

```bash id="h1"
ssh username@ip_address
```

### 🧪 Example

```bash id="h2"
ssh user@192.168.1.1
```

---

## 📦 9. Create Files & Move

### ❓ Question

Create two files and move them into another directory.

### 💡 Explanation

Use `touch` and `mv`.

### ⚙️ Syntax

```bash id="i1"
touch file1 file2
mv files destination
```

### 🧪 Example

```bash id="i2"
touch a.txt b.txt
mkdir newDir
mv a.txt b.txt newDir/
```

---

## 💽 10. Check Disk Usage

### ❓ Question

Check disk usage of a directory.

### 💡 Explanation

Use `du`.

### ⚙️ Syntax

```bash id="j1"
du -sh directory
```

### 🧪 Example

```bash id="j2"
du -sh mainDir
```

---

## 📜 11. Command History

### ❓ Question

Display command history.

### 💡 Explanation

Use `history`.

### ⚙️ Syntax

```bash id="k1"
history
```

### 🧪 Example

```bash id="k2"
history
```

---

## 🌍 12. Verify Connectivity

### ❓ Question

Verify connectivity to a website.

### 💡 Explanation

Use `ping`.

### ⚙️ Syntax

```bash id="l1"
ping domain
```

### 🧪 Example

```bash id="l2"
ping google.com
```

---

## 📂 13. Directory + Files + Display Content

### ❓ Question

Create a directory `lab1`, create two files and display contents.

### 💡 Explanation

Use `mkdir`, `touch`, `cat`.

### ⚙️ Syntax

```bash id="m1"
mkdir directory
touch file
cat file
```

### 🧪 Example

```bash id="m2"
mkdir lab1
touch lab1/file1.txt lab1/file2.txt
cat lab1/file1.txt
```

---

## 📋 14. Copy File & Verify

### ❓ Question

Copy a file from one location to another and verify.

### 💡 Explanation

Use `cp` and `ls`.

### ⚙️ Syntax

```bash id="n1"
cp source destination
ls
```

### 🧪 Example

```bash id="n2"
cp file.txt /home/user/
ls /home/user/
```

---

## 🖥️ 15. System Name & Kernel Version

### ❓ Question

Display system name and kernel version.

### 💡 Explanation

Use `uname`.

### ⚙️ Syntax

```bash id="o1"
uname -a
```

### 🧪 Example

```bash id="o2"
uname -a
```

---

## 🛰️ 16. Traceroute Command

### ❓ Question

Trace the path taken by packets to reach a destination.

### 💡 Explanation

`traceroute` shows the **route (hops)** that data travels from your system to a destination.
Useful for **network troubleshooting**.

### ⚙️ Syntax

```bash id="p1"
traceroute domain_or_ip
```

### 🧪 Example

```bash id="p2"
traceroute google.com
```

### 📌 Output Meaning

* Each line = one **hop (router)**
* Shows **IP address + time (ms)**
* More hops → longer route

### ⚠️ If Not Installed

```bash id="p3"
sudo apt install traceroute
```

### 💡 Alternative

```bash id="p4"
tracepath google.com
```

---
