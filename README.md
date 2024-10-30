![image](https://github.com/user-attachments/assets/b4466603-7b93-4e37-96cf-669b9964f49f)


<h1>Elasticsearch Setup</h1>
This tutorial demonstrated the installation of elasticserach.<br />


<h2>Environments and Technologies Used</h2>

- VULTR Cloud Computing
- Ubuntu 22.04 x64
- Powershell <br />

<h3>Spin up a Ubuntu VM on VULTR and SSH into it using Powershell</h3>

![Screenshot 2024-10-29 212253](https://github.com/user-attachments/assets/06d7b5bc-afac-428f-8ff3-118618c772f7) <br />

<h3>Update repositories</h3>

using "apt-get update && apt-get upgrad -y"

![Screenshot 2024-10-29 212443](https://github.com/user-attachments/assets/c6de4c7d-49aa-41b0-be97-704ba0e02da0) <br />

<h3>Download Elasticsearch</h3>

![Screenshot 2024-10-29 212651](https://github.com/user-attachments/assets/387cd86f-9ed0-4449-96ea-18b9123be6d7)

After the download is complete, use the command "dpkg -i elasticsearch-8.15.3-amd64.deb" to install elasticsearch. 

![Screenshot 2024-10-29 212749](https://github.com/user-attachments/assets/2407d704-6af5-4cf0-8359-5d6b5a559a4b) <br />

<h3>Elasticsearch Configuration File</h3>

The elasticsearch configuration file (elasticsearch.yml) can be found in /etc/elasticsearch. Use nano to change the network configuration to your IP address. 

![Screenshot 2024-10-29 213053](https://github.com/user-attachments/assets/ecbf665f-bbba-4842-9f33-d40105ba3342)

![Screenshot 2024-10-29 213257](https://github.com/user-attachments/assets/0fab50c7-1b90-4003-9d98-a767a161fc12)

![Screenshot 2024-10-29 213354](https://github.com/user-attachments/assets/4b5a0953-6001-4007-855d-9dcc47c3aae1)

![Screenshot 2024-10-29 213545](https://github.com/user-attachments/assets/74ae273e-8ed4-4a26-87b4-3f31daad6b74) <br />

<h3>Startup the Elasticsearch Service</h3>

Use the following commands:

- systemctl daemon-reload
- systemctl enable elasticsearch.service
- systemctl start elasticsearch.service
- systemctl status elasticsearch.service 

![Screenshot 2024-10-29 214015](https://github.com/user-attachments/assets/64a80f24-88fc-45d9-a743-b395e21c0b8b)



