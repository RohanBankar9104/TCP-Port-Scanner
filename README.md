# 🌐 TCP Port Scanner

A high-performance multithreaded TCP Port Scanner built in Python that efficiently scans a target host for open, closed, and filtered ports. The scanner utilizes socket programming and concurrent threading to accelerate the scanning process while maintaining reliable results and automatic logging.

---

## 📌 Overview

Port scanning is one of the most fundamental techniques used in networking and cybersecurity to identify open services running on a system.

This project demonstrates how TCP port scanning works by attempting TCP connections to a specified range of ports and reporting their status. The application uses multithreading to significantly improve scanning speed and automatically stores results for later analysis.

---

## 🚀 Features

* ⚡ Fast multithreaded scanning
* 🌐 Hostname and IP address support
* 🔍 Custom port range selection
* 📊 Real-time scan results
* 📝 Automatic result logging
* ⏱ Timeout handling
* 🛡 Error handling and validation
* 📂 Results exported to text file

---

## 🏗️ How It Works

The scanner follows these steps:

1. User enters a target hostname or IP address.
2. Hostname is resolved into an IP address.
3. Multiple worker threads are created.
4. Ports are added to a task queue.
5. Each thread attempts a TCP connection.
6. Port status is determined:

   * OPEN
   * CLOSED
   * TIMEOUT
7. Results are displayed and saved to a log file.

---

## 🛠️ Technologies Used

| Technology         | Purpose                  |
| ------------------ | ------------------------ |
| Python             | Core Development         |
| Socket Programming | Network Communication    |
| Multithreading     | Concurrent Port Scanning |
| Queue Module       | Task Management          |
| Datetime Module    | Performance Tracking     |

---

## 📂 Project Structure

```text
TCP-Port-Scanner/
│
├── PortScanner.py
├── scan_results.txt
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/RohanBankar9104/TCP-Port-Scanner

cd TCP-Port-Scanner
```

### Verify Python Installation

```bash
python --version
```

Python 3.x is required.

---

## ▶️ Usage

Run the scanner:

```bash
python PortScanner.py
```

### Example

```text
Enter target host/IP: scanme.nmap.org
Start Port: 1
End Port: 1000
```

Output:

```text
Port 22    : OPEN
Port 80    : OPEN
Port 443   : OPEN
Port 8080  : CLOSED
```

---

## 📸 Sample Output

```text
============================================================
TCP Port Scanner
============================================================

Target: scanme.nmap.org
IP: 45.33.32.156

Scanning Ports: 1 - 1000

Port 22    : OPEN
Port 80    : OPEN
Port 443   : OPEN

============================================================
Scan Complete
============================================================
```

---

## 📝 Logging System

All scan results are automatically saved to:

```text
scan_results.txt
```

Example:

```text
Port 22    : OPEN
Port 80    : OPEN
Port 443   : OPEN
```

This allows users to review results after the scan is completed.

---

## 🎯 Learning Objectives

This project helped develop practical knowledge in:

* TCP/IP Networking
* Port Scanning Techniques
* Socket Programming
* Concurrent Programming
* Multithreading
* Queue Management
* Network Security Fundamentals

---

## 📈 Performance Features

The scanner uses:

* 100 concurrent worker threads
* Queue-based task management
* TCP connection testing
* Timeout controls

These optimizations significantly reduce scanning time compared to a single-threaded implementation.

---

## 🔮 Future Improvements

* UDP Port Scanning
* Service Version Detection
* Banner Grabbing
* Operating System Detection
* CSV Export Support
* JSON Report Generation
* GUI Interface (Tkinter/PyQt)
* Vulnerability Detection Module

---

## ⚠️ Disclaimer

This tool is intended for educational purposes and authorized security testing only.

Always obtain proper authorization before scanning any network, server, or device that you do not own or have permission to assess.

Unauthorized scanning may violate laws, regulations, or organizational policies.

---

## 👨‍💻 Author

### Rohan Bankar

Cybersecurity Enthusiast | Networking Learner | VAPT

---

## 📄 License


Feel free to use, modify, and distribute it for educational and learning purposes.
