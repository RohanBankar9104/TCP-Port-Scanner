A fast and efficient multithreaded TCP Port Scanner developed in Python. This tool scans a specified range of ports on a target host and identifies whether ports are open, closed, or timed out. Scan results are displayed in real time and automatically saved to a log file.

-Features-
1.Multi-threaded scanning for improved speed
2.Custom port range selection
3.Hostname and IP address support
4.Real-time scan results
5.Automatic logging to scan_results.txt
6.Socket-based TCP connection testing
7.Error and timeout handling
8.Technologies Used
9.Python 3
10.Socket Programming
11.Multithreading
12.Queue Management

--How It Works--

-The scanner:

1.Resolves the target hostname to an IP address.
2.Creates multiple worker threads.
3.Assigns ports to threads using a queue.
4.Attempts TCP connections to each port.
5.Reports whether ports are:
                            OPEN
                            CLOSED
                            TIMEOUT
6.Saves results to a log file.

--Installation--
git clone https://github.com/RohanBankar9104/TCP-Port-Scanner

--Usage--
python PortScanner.py

-Example:

Enter target host/IP: scanme.nmap.org
Start Port: 1
End Port: 1000
Output Example
Port 22    : OPEN
Port 80    : OPEN
Port 443   : OPEN
Port 21    : CLOSED

Results are automatically saved to:

scan_results.txt
Project Structure
TCP-Port-Scanner/
│
├── PortScanner.py
├── scan_results.txt
└── README.md
Future Improvements
UDP Port Scanning
Service Version Detection
Banner Grabbing
Export Results to CSV/JSON
GUI Interface using Tkinter or PyQt
OS Detection
Custom Thread Configuration
Learning Outcomes

This project helped strengthen understanding of:

TCP/IP Networking
Socket Programming
Multithreading in Python
Queue-based Task Management
Port Scanning Methodology
Cybersecurity Fundamentals


--Disclaimer--

This tool is intended for educational purposes and authorized security testing only. Always obtain proper permission before scanning any network or system.


