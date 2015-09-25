SIPFLANKER USER’S MANUAL


Many  (if not most) VoIP devices have available a Web GUI for their configuration,
management, and report generation. These Web GUIs are often on default, meaning that
the moment you install the IP phone or IP PBX, the Web GUI is immediately available
on the network. And unfortunately it is also common for the username and password
to have the default values.

Sipflanker will help you find these SIP devices with potentially vulnerable Web GUIs
in your network.

What the application does is search the range of IPs you specify, and checks if port
5060 is available. Whether open or close, port 5060 indicates the presence of a SIP
device. Then it checks if port 80 (http) is open. The combination of an open port 80,
together with port 5060, either open or closed, signals a SIP device with a Web GUI.

Sipflanker then proceeds to extract the website, and fingerprint the device.
You can find default passwords for IP phones at http://www.infosegura.net/passwords.htm

Sipflanker runs on Python, so you need to have it installed. You can download it at
http://www.python.org/download/

To use Sipflanker, simply enter the Windows DOS shell, navigate to the folder where
you placed sipflanker.py, and type “sipflanker.py”. Enter the IP, or use the format
xxx.xxx.xxx.0-100 Using “-“ to indicate ranges. Presently only C networks can be searched.


The scan results will be desplayed on the screen, and also written to the file
flank.txt, present in the same folder where sipflanker.py resides.

If  you have any questions or comments, you can contact me at sergio[at](at.md)infosegura.net.