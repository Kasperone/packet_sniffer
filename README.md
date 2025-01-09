# Packet Sniffer

This is a Python script that demonstrates HTTP packet sniffing on a network interface. It captures HTTP requests and extracts potential login information, such as usernames and passwords, for educational and ethical hacking purposes.

## Features
- Captures HTTP requests on a specified network interface.
- Extracts and displays requested URLs.
- Identifies potential login credentials (e.g., usernames and passwords) from HTTP packets.

## Prerequisites
- Python 3.x
- Linux-based operating system
- `scapy` library (for handling network packets)

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/packet_sniffer.git
cd packet_sniffer
```

Install the required library:

```bash
pip install scapy
```

## Usage

Run the script with superuser privileges to start sniffing packets on a specified network interface.

```bash
sudo python3 packet_sniffer.py
```

### Notes:
- Replace `eth0` in the script with the name of the network interface you want to monitor (e.g., `wlan0` for Wi-Fi).
- The script only captures HTTP traffic; it does not work with HTTPS traffic, as HTTPS encrypts its content.

## Example:

Run the script to sniff packets on the `eth0` interface:

```bash
sudo python3 packet_sniffer.py
```

Output:

```
[+] HTTP Request >> example.com/index.html

[+] Possible username/password > username=admin&password=1234
```

## Notes:
- This script is for educational purposes only. Use it responsibly and only in environments where you have permission to perform testing.
- HTTPS traffic cannot be captured or decrypted by this script.

## Troubleshooting:
- Ensure you have the required libraries installed.
- Make sure to run the script with `sudo` or as root to access network packets.
- Verify that you are monitoring the correct network interface.

## License
This project is licensed under the MIT License.

## About

This script is part of the course [Learn Python & Ethical Hacking from Scratch](https://www.udemy.com/course/learn-python-and-ethical-hacking-from-scratch/) on Udemy. The course covers Python scripting and its application in ethical hacking, network security, and more.
