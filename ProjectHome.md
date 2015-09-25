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

http://www.infosegura.net/