# Cloud-SOC-Lab-with-Wazuh
Built and configured a Cloud-based SOC lab using Wazuh XDR/SIEM

What is Wazuh? 

**Answer**: - Wazuh is an open-source security platform with XDR & SIEM capabilities. It protects systems across on-premises, virtualized, containerized, and cloud-based environments. 

•	Monitoring 
•	Alerting
•	Compliance

To Start, we go to wazuh.com

![image](https://github.com/user-attachments/assets/aca90b7b-fdbb-4319-8ea4-620883073244)

We click on Free Cloud Trial since we are using the Cloud. It looks like this below

![image](https://github.com/user-attachments/assets/4cd6427d-36e3-4097-bc25-dd3167334e6d)

After creating an account with a student or business email, the dashboard should look like this.

![image](https://github.com/user-attachments/assets/4bd39e67-6518-4208-a654-a6a7a2acb794)

Click Start your free trial to create your environment. It should look like this

![image](https://github.com/user-attachments/assets/d4dbc050-7507-4996-883e-25658a1f26a7)

Keep everything as default. After that, your page will look like this 

![image](https://github.com/user-attachments/assets/b146007e-ff33-43db-8162-6a1fcb951d04)

We can open Wazuh by clicking on the top right and it should look like this

![image](https://github.com/user-attachments/assets/238b74cc-c9e2-46af-80ec-d20f7f8db2a8)

To get the Username and password, go to the top right closer Wazuh and click Manage, scroll down and click on Default Credentials

![image](https://github.com/user-attachments/assets/1c6a4fd0-2f83-4fe4-b727-173e7c415d28)

**Wazuh Dashboard**

![image](https://github.com/user-attachments/assets/5bd9365d-8379-4e1e-b75a-9e2bc1453885)

Now let add some agents. And for this project, we will use a linux machine.

![image](https://github.com/user-attachments/assets/77c08e50-2219-4880-849d-cf35d13a3fbf)

For some reason the Agent wasn’t going through, and I asked ChatGPT about it and he help me out. Since we are using a Windows Ubuntu (WSL) we should run it without systemd. To verify if we are using systemd, we run the ps -p 1 -o comm= command and it shows we are not in systemd but init.

•	After that, we run this sudo /var/ossec/bin/wazuh-control start command to install Wazuh and it work.

![image](https://github.com/user-attachments/assets/8a8ca4a9-6df3-4117-b7ba-62e2c816a5a9)

**Agent Dashboard:**

![image](https://github.com/user-attachments/assets/e177a520-4a71-41bd-bedb-58103ca398b3)





