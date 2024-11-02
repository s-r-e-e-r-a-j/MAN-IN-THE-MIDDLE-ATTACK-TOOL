This Is A arp poisoning  Man In The Middle Attack Tool Maded With Python Language

installation 


Clone the respository:-


```git clone https://github.com/s-r-e-e-r-a-j/MAN-IN-THE-MIDDLE-ATTACK-TOOL.git```

```cd MAN-IN-THE-MIDDLE-ATTACK-TOOL```

```cd 'MITM TOOL' ```

  Run the command ```pip install -r requirements.txt``` to install all the packages required in your virtual environment.

Run This Tool on kali linux or other hacking os by Executing :

```sudo python3 arp_mitm.py  -ip_range 192.168.1.0/24 ```


if any module is missing install it by executing
```pip3 install misssingmodulename``` on terminal

if you run this tool in kali linux or other hacking os on desktop by executing``` python3 arp_mitm.py  -ip_range 192.168.1.0/24 ```it will display Ip Address of all the devices connected to your wifi network.then select a device for attack by its
id then the arp poisoning will start if you want to stop press ```ctrl+c ```.then all the result will be stored in a pcap file named requests.pcap on Desktop.then open it on wireshark to analyse the received packets
