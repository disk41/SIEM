# SIEM

                                                       WAZUH  
Go to https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html
 Click this link https://packages.wazuh.com/4.x/vm/wazuh-4.3.4.ova to download the virtual machine.
Open downloaded file with VirtualBox by right click and open with VirtualBox . 
It will automatically set according to their requirement and then click on import to proceed.
After installing, the machine has to be started.




![image](https://user-images.githubusercontent.com/67914237/173249260-d7c3a579-3cac-4f75-baf8-d7dcd00b3bde.png)
















Let's start to see the machine terminal and determine the IP where we will reach wazuh web interface.
So the virtual machine is booting up. 



![image](https://user-images.githubusercontent.com/67914237/173249270-0b0fd132-371e-4aa6-afcc-b6ec32112693.png)









The wazuh-server login is ' root' and the password is ' wazuh ' which was mentioned in the documentation.










![image](https://user-images.githubusercontent.com/67914237/173249284-15cee270-8e55-4c65-8a1a-533787dbe5d7.png)








Once logged in we can determine the IP address of the system by typing in' ip addr '. I note that the IP address in this case will be ' 192.168.43.59 ‘







![image](https://user-images.githubusercontent.com/67914237/173249297-07d1b656-e999-4a1f-8829-02711e6deae4.png)














Then we need to press the right control key to release our mouse pointer. We can then direct our browser to access the Web Interface at ' https://192.168.43.59   '. 








![image](https://user-images.githubusercontent.com/67914237/173249311-9769eb3e-e694-4f49-831f-938d1a2002cd.png)











There will be a warning that the certificate used by the OVA is not signed by a trusted authority. We ignore and continue to 192.168.43.59(unsafe) for testing purposes. 






![image](https://user-images.githubusercontent.com/67914237/173249329-0ea0bf82-e0ee-49f9-8e41-cf913538a3d4.png)













Then here on the web page, we will have to give the user ID and password.
User id - admin and Password- admin.










![image](https://user-images.githubusercontent.com/67914237/173249338-ede1d568-daa0-4f3d-979b-b54dd6b7c789.png)









The web page will now load the Kibana Web Interface and on the left-hand column,we will find the Wazuh icon that will take us to the Wazuh Web Interface with Kibana.









![image](https://user-images.githubusercontent.com/67914237/173249346-4d4628c4-efc3-4da0-86cb-e949dc3323e6.png)















There we will have access to the dashboard of the Wazuh. We can see that no agents have been registered to this manager. If we click on the Add agents link or on the Agent tab. We will be directed to the interface which will provide guidance on how to deploy Wazuh agents on several operating systems . 







![image](https://user-images.githubusercontent.com/67914237/173249361-63c5026a-86e4-4b69-80e6-f5f989ee3994.png)












We can select Windows and provide the IP address where we can find the Wazuh manager. This will provide us with a command that we can copy and paste onto our systems to download, install, register and configure the Wazuh agent without any further interaction.







![image](https://user-images.githubusercontent.com/67914237/173249372-8daf7567-c03e-4c87-a225-2e92c9923a84.png)











Let's bring a terminal with Windows11 machine and paste that command into it to see how it works.Just hit enter and confirm the action, it's as simple as that.






![image](https://user-images.githubusercontent.com/67914237/173249385-7e5538b0-4703-40d6-9a9e-1e5d008a582c.png)













This works not only on Windows but also on centOS, MacOS, another Linux system. We can now reload the agents tab to see our newly registered endpoint being monitored.







![image](https://user-images.githubusercontent.com/67914237/173249395-f79d06e5-b82b-4f41-b3a4-a947ca3bb1b8.png)



![image](https://user-images.githubusercontent.com/67914237/173249412-a262559f-a8ae-4a75-828b-4c7d18691db7.png)






![image](https://user-images.githubusercontent.com/67914237/173249422-da2d2ee5-fe2a-4798-9ba7-a45461a8ce95.png)


We can then explore the interfaces by going on to overview and select a dashboard to visualize the events being logged by the system. If we go to discover more we may see all the details of any of the registered events.

 Click "Agents" to view your agents.
 Click "Overview" and then click "Security Events" to view the agent's monitoring events. 
 Click "Discover" to review any registered events





