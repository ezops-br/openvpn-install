# How to use
### ⚠️ This script work with Ubuntu 20.04.0 ami ⚠️

- Upload vpn template to cloudformation
- Click on the "resources" tab, on the cloudformation stacks page, then on the AutoScalingGroup link

![screenshot01](./screenshots/screen01.png)
- Then click on "instance management", choose the VPN instance and click on it

![screenshot02](./screenshots/screen02.png)

- Then click on the connect button and choose the best option to connect to the instance. In this example, we will connect to EC2 directly through the AWS platform. Then click in connect orange button

![screenshot03](./screenshots/screen03.png)
![screenshot04](./screenshots/screen04.png)

- A terminal will open inside the instance on another screen, similar to the picture below:

![screenshot05](./screenshots/screen05.png)

- We need to get the vpn client file generated, then run the "ls" command

- With the client.ovpn file generated, we need to copy its content to a file on our local machine, for that we will issue the command "cat client.ovpn". And this is the result:

![screenshot06](./screenshots/screen06.png)
![screenshot07](./screenshots/screen07.png)

- The content must be copied to an external file with the ".ovpn" extension. After that, we need to test the connection to the VPN, for that we will use the "OpenVPN Connect" program. Tool download link [here( for windows)](https://openvpn.net/client-connect-vpn-for-windows/)

![screenshot08](./screenshots/screen08.png)

- After installing the tool, open the program and click on the file tab. Then import the file with the client content and click on connect, like the images below:

![screenshot09](./screenshots/screen09.png)
![screenshot10](./screenshots/screen10.png)

- VPN connected

![screenshot11](./screenshots/screen11.png)