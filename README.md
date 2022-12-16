# UDP-Scripts-Unity
Simple Sender and Receiver Scripts for UDP messages in Unity

How to Use:
- If you already have an "Empty" game object in the scene which you are using as a Manager, attach both the scripts to that. If not, then create a new empty game object in the scene and then attach both the scripts to that.

UDP Sender:
- "Data to Send" - Takes the message to send. Edit the text or change the data being sent
- "IP" - The IP address of the machine which has a UDP listener on it. Think of this as the house address. Get it using ipconfig/ifconfig in Windows/Linux machines
- "TxPort" - The port on which the other machine is listening. Think of it as the one of the doors to the house. Set it to some number higher than 5000.

When you hit "Space Bar" in the game after running it, it will send the above message

UDP Receiver:
- "RxPort" - The port on which you want this machine to listen to for UDP messages. The sending machine should be sending messages on this port.


Note: If you are able to send UDP messages but not able to receive them, then the culprit is most likely your firewall. Add Unity to it and allow inbound connections.
