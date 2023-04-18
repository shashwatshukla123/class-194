# class-194
IP and mac ; switches connection.
*Commands to run in cmd*
ipconfig[for windows] ,ifconfig[for mac & linux]: To get ip address of your computer.
ipconfig/all: To get mac address of device.
nslookup x.com : To get the ip address of the x website. 

------------------------------------------------------------------------------------------------------

We can clear the cmd by using the cls command.
---------------------------------------------------------------
MAC stands for Media Access Control.

It is a set of 12 digits,
 the first 6 digits refer to the manufacturer of the device
The rest of the 6 digits are the ones which are unique for each device. 

The IP address is a unique set of numbers assigned to a computer on a network.
MAC Address is permanent whereas an IP Address can change.

To see the mac address of our computer we can simple
type a command in the command prompt as ipconfig /all
(Ifconfig /all for mac os).
Here you will see a lot of information. The mac address is
called a physical address.
But you can that we have multiple mac addresses here.
This is because each networking device in the computer
has a mac address.
The computer has an ethernet device, which helps us to
connect with networking using a LAN cable.
Then we have a wifi module and bluetooth module as well.
So all of these devices are assigned a mac address.

Wireless Lan adapter wi-fi
This is the mac address of the wifi module of my computer.
The Mac address is a 12 digit hexadecimal number
The first 6 digits of the mac address tells us about the
manufacturers. So these will be the same for all the
devices made by that manufacturer.
Rest of the 6 digits are unique for each device.
2 devices can not have the same mac address.

---------------------------------------------------------------------

switch was a device which can work like an extension device, to provide us with a number of ports where we can connect other computers

Switch is a networking device which helps us to connect multiple devices together and forms a LAN (Local Area Network).

A switch is a networking device which receives a message from any device in the network and transmits it only to the device for which it was meant. The switch does this by storing the MAC addresses of the devices which are connected to the network. Then, when a message is to be delivered to a specific device on the network, it compares the MAC address written on the message with the MAC addresses of the devices. Then it sends the message to the specific device whose MAC address was mentioned on the message.

———————————————————
To connect the computer with Switch click on the computer and then click on the switch. We need to do this for the 2 other computers.
————————————————————

The next step is to assign the ip address to the computers and perform a ping test.
——————————————————
Now we will add one more computer on our screen and connect that with the switch.

To connect this with the switch we will not use the automatic connection we are going to choose the cable manually. And the cable is called copper straight through cable.

This will give the options of the port where we want to connect this cable. While creating the network we will always connect the cable with a fast ethernet port.Because this the port reserved for networking. On this computer it is FastEThernet0. Select this option and then click on the switch

Switch has many ethernet ports. To connect multiple computers. When you click on the switch it shows the available port for the connection. First 3 ports are used by the first 3 computers. So we will choose the FastEthernet port 4.

This happens because the switch takes some time to set up and while it is showing an orange circle it means that the setup is not complete. Usually this turns into green in less than a minute. But since we are in a simulation we can make it fast. By clicking on the fast forward button.


——————————————
Select the packet and you can see there is an envelope icon on the cursor. 

This is a data packet.

 Once you select the data packet then click on the first computer and then click on the 4th computer. 

What we are doing here is sending data from the first computer to the 4th one. It is just like doing a ping. Select the packet and then click on the first pc and then on the 3rd PC. This will show a message icon on the first PC.


Now the packet is at the first PC, in order to move it forward we need to click on the forward button in the bottom menu. When you click on that button it will send the packet to the switch and to the packet forward you need to click that button again. Which will send the packet to the target PC.

——————————————————

There used to be a device named HUB. 
f you are sending the data from the computer to another computer via the hub. It used to send that data to each and every computer. 

Which is not an ideal scenario. Because we want to send data to only 1 computer. That is where the switch comes into the picture.

Switch stores the MAC address of the device and it sends the data to that device only. We can see the mac address stored in the switch by running a very simple command. 

But first double click on the switch. Then select the CLI option. This stands for command line interface. This is similar to the command prompt. We can run the commands here.
—————————————

The command we are going to run is show mac-address-table this will show all the mac address stores in the switch.Type this command and press enter.

show mac-address-table 

This shows the mac address of the first and 3rd PC, because we did a ping between these two computers only. To register the Mac address in the switch we need to ping the device. We can check whether these MAc addresses are correct or not by comparing them with the mac address of the first and 3rd PC. Take the cursor on the PC and hold it there it will show the mac address.

Here it shows the 2 mac addresses for each PC. That is because each networking device in the computer is assigned a mac address. So the first mac address is an ethernet device with which our computer is connected with a switch. The second mac address here is of the bluetooth device on the computer. When we checked the mac address of our computer we saw multiple mac addresses associated with different networking devices on our computer.
