# 🐍 Python — Open Source Audit Project

> A capstone project exploring the internals and ecosystem of **Python**, one of the world's most beloved open source languages — through a suite of Linux shell scripts.

---

## 👤 Developer Info

| Field | Details |
|---|---|
| **Student Name** | Basavanneppa Shiwalingappa Mugad |
| **Registration Number** | 24BCY10322 |
| **Chosen Software** | Python |

---

## 📁 Project Structure

```
open-source-audit/
├── sys_identity.sh       # System information reporter
├── package_inspector.sh  # Package detection & FOSS descriptions
├── disk_auditor.sh       # Directory size & permissions auditor
├── log_analyzer.sh       # Log file keyword analyzer
└── manifesto.sh          # Interactive philosophy manifesto generator
```

---

## 🛠️ Script Overview

### 1. `sys_identity.sh` — System Identity Reporter
Displays key system information using basic variables and command substitution.

**Reports:**
- Kernel version
- OS distribution
- Currently logged-in user
- System uptime

---

### 2. `package_inspector.sh` — Package Inspector
Checks whether `python3` is installed and echoes a philosophical description of various FOSS packages.

**Features:**
- Detects package manager (`dpkg` / `rpm`)
- Uses a `case` statement for FOSS package descriptions

---

### 3. `disk_auditor.sh` — Disk Auditor
Iterates through a predefined array of directories and reports their disk usage and permissions.

**Uses:** `ls -ld`, `awk`, `du`

---

### 4. `log_analyzer.sh` — Log File Analyzer
Reads a log file line-by-line using a `while read` loop to count and surface keyword occurrences.

**Usage:**
```bash
./log_analyzer.sh <log_file_path> <keyword>
```
**Example:**
```bash
./log_analyzer.sh /var/log/syslog error
```

**Output:**
- Total count of keyword matches
- Last 5 matching lines

---

### 5. `manifesto.sh` — Open Source Manifesto Generator
An interactive script that asks the user three questions and writes a personalized Open Source Philosophy manifesto to a `.txt` file.

---

## 🚀 Getting Started

### Prerequisites
- A Linux environment with a standard Bash shell (`/bin/bash`)
- Common utilities (pre-installed on most distros): `awk`, `cut`, `grep`, `tail`, `du`, `dpkg` or `rpm`

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/open-source-audit.git
cd open-source-audit

# 2. Grant execute permissions to all scripts
chmod +x *.sh
```

### Running the Scripts

```bash
# System identity
./sys_identity.sh

# Package inspector
./package_inspector.sh

# Disk auditor
./disk_auditor.sh

# Log analyzer (requires a log file path and keyword)
./log_analyzer.sh /var/log/syslog error

# Manifesto generator
./manifesto.sh
```

---

## 📦 Dependencies

No additional installation required. All dependencies are standard Linux utilities available out-of-the-box on mainstream distributions.

| Tool | Purpose |
|---|---|
| `bash` | Script interpreter |
| `awk` | Text processing |
| `grep` | Pattern matching |
| `cut` | Field extraction |
| `tail` | Last N lines of output |
| `du` | Disk usage |
| `dpkg` / `rpm` | Package inspection |

---

## 📜 License

This project was created for academic purposes as part of a capstone assignment. Feel free to reference or adapt it for educational use.

---

<p align="center">Made with ❤️ and <strong>Bash</strong> — in the spirit of open source</p>
