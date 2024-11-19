


## MITM Tool - ARP Poisoning & Packet Sniffing
MITM Tool is a Python-based network security tool for performing ARP (Address Resolution Protocol) poisoning attacks, commonly known as Man-in-the-Middle (MITM) attacks. It intercepts network traffic between a target client and the network gateway. The tool is designed for educational purposes and authorized penetration testing only.

## Features
- **ARP Scanning**: Automatically discovers devices on the network and their IP/MAC addresses.
- **ARP Spoofing**: Spoofs ARP packets to redirect traffic through the attacker's machine.
- **Packet Sniffing**: Captures all intercepted packets and saves them as .pcap files for analysis.
- **Multithreading**: Runs ARP spoofing and packet sniffing simultaneously.
- **User Interface**: Displays a list of available devices and allows the user to select a target device for ARP poisoning.
## Requirements:
- **Python 3.x**
- **Scapy (Python library for packet manipulation)**
- **Root (sudo) privileges to run the script**
- **Linux-based OS (Tested on Kali Linux)**
## Installation
1.  **Install Dependencies:**
 
`Ensure you have Python 3.x installed `
```bash
pip3 install -r requirements.txt
```

2 . **Clone the Repository:**

Clone this repository to your local machine.

``` bash
git clone https://github.com/s-r-e-e-r-a-j/MITM-TOOL.git
```
```bash
cd MITMTOOL
```
```bash
cd 'MITM TOOL'
```
## Usage
1. **Run the Tool:**

To run the tool, use the following command with the desired IP range:

```bash

sudo python3 arp_mitm.py -ip_range 192.168.1.0/24
```
Replace 192.168.1.0/24 with the IP range of your target network.

2.  **Menu Interaction:**

Once the tool starts, it will display a list of devices found in the network and their IP/MAC addresses. You will then be prompted to select a target device for ARP poisoning.

**Example output:**

```markdown
ID      IP                MAC Address
------------------------------------------
0       192.168.1.2       00:1a:2b:3c:4d:5e
1       192.168.1.3       00:1b:2c:3d:4e:5f
2       192.168.1.4       00:1c:2d:3e:4f:60
```
Choose the ID of the device whose ARP cache you want to poison.

3. **Capture Packets:**

Once ARP poisoning is active, all intercepted packets will be saved in a `requests.pcap` file in `'MITM TOOL'` Directory, which can be analyzed using Wireshark.

4. **Stop the Tool:**

To stop the script, simply press Ctrl + C.

## Important Notes
- **Legal Disclaimer**: This tool is intended for educational purposes only. Do not use it on any network without explicit permission from the network owner. Unauthorized use of this tool is illegal and can result in severe consequences.
- **Root Privileges**: The script requires root (sudo) privileges to interact with network interfaces and manipulate ARP tables.
- **Network Disruption**: The tool can disrupt normal network traffic for both the target and the attacker’s machine. Use it responsibly in controlled environments.

## Example Workflow
1. **Run the tool with the desired IP range:**

```bash
sudo python3 arp_mitm.py -ip_range 192.168.1.0/24
```
2. **Select a device to target (ARP poisoning):**

``` vbnet
Please select the ID of the computer whose ARP cache you want to poison (ctrl+z to exit): 1
```
3. **The script will begin ARP poisoning, sending spoofed ARP packets, and sniffing network traffic.**

4. **Intercepted packets are saved in `requests.pcap` on `'MITM TOOL'` Directory and can be analyzed in Wireshark.**


## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer: 
Use this tool responsibly. Unauthorized usage is illegal and unethical. Always obtain permission before testing any network.






