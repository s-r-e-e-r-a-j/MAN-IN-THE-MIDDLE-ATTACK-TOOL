# This Is A arp poisoning  Man In The Middle Attack Tool Maded With Python Language

# installation 


# Clone the respository:-


```bash
git clone https://github.com/s-r-e-e-r-a-j/MITM-TOOL.git
```

```bash
cd MITM-TOOL
```

```bash
cd 'MITM TOOL'
 ```

## install requirements(optional if you are using kali linux):-

` In kali linux all requirements for this tool  are pre-installed on it.requirements means the packages required for this tool to work.so don't need to install requirements for this tool on kali linux`

```bash
pip3 install -r requirements.txt
```


 Run This Tool on kali linux or other hacking os by Executing :

```bash
sudo python3 arp_mitm.py  -ip_range 192.168.1.0/24
 ```


if any module is missing install it by executing
```bash
pip3 install misssingmodulename
```
 on terminal

 if you run this tool in kali linux or other hacking os on desktop by executing
```bash
python3 arp_mitm.py  -ip_range 192.168.1.0/24
```
 it will display Ip Address of all the devices connected to your wifi network.then select a device for attack by its id then the arp poisoning will start if you want to stop press ```ctrl+c ```.then all the result will be stored in a pcap file named requests.pcap on Desktop.then open it on wireshark to analyse the received packets
