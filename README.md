<H1>Azure Cloud Detection Using Sentinel</H1>

<h2>Description</h2>
In this lab I will configure and Deploy Azure Resources such as Virtual Machines and Microsoft Sentinel. Demonstrate and configure windows security policies and event logs as well as best practices. Utilize Data Connectors to bring data into Sentinel for Analysis.
<br />


<h2>Languages and Utilities Used</h2>

- <b>KQL</b>
- <b>MITRE</b>


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>
- <b>Microsoft Sentinel</b>

<h2>Program walk-through:</h2>

<p align="center">
Create a resource group: <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/5970b9c9-7043-416e-aaa7-c63794b61304

<br />
<br />
<p align="center">
Create a Virtual Machine:  <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/43b9e517-1f1a-4922-b636-338c19cdd045

<p align="center">
<ins>It will take a moment and then you should see this:</ins> <br/>
<img src="https://i.imgur.com/kreBoa3.jpeg" height="" width="70%" />

<br />
<br />

<p align="center">
<ins>Enable Microsoft Defender for Cloud:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/eec687bf-e220-46d9-bd54-4a539fa66e0a


<br />
<br />

<p align="center">
<ins>We want to configure Just in Time Policy:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/a7bfa792-dc5c-415e-a851-ca2367a5f1ca

<br />
<br />


<p align="center">
<ins>Then we make sure to set our connection rule:</ins> <br/>
<img src="https://i.imgur.com/xsUmwFW.jpeg" height="" width="70%" />
<p align="center">
<ins>Confirm:</ins> <br/>
<img src="https://i.imgur.com/i2c66NJ.jpeg" height="" width="70%" />


<br />
<br />



<p align="center">
<ins>Create Microsoft Sentinel Workspace:</ins> <br/>



https://github.com/IsaacPerezCyber/SIEM/assets/67014769/fd9a699a-1eb8-4118-92d0-bb9514b397a6



<br />
<br />

<p align="center">
<ins>Configure data collection rule for log integration in Microsoft Sentinel:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/eb745ca2-7577-4f93-a906-1a961536bf4f

<br />
<br />

<p align="center">
<ins>We make sure to confirm the log connection:</ins> <br/>
<img src="https://i.imgur.com/QovmfgQ.png"  width="70%" />

<br />
<br />

<p align="center">
<ins>Now we RDP into the VM to generate traffic on the Sentinel Logs:</ins> <br/>
<img src="https://i.imgur.com/ttFTvOB.jpeg" height="" width="70%" />


<br />
<br />

<p align="center">
<ins>Check security logs in the remote machine to verify a successful logon:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/20ab1ef0-d3cd-48f9-8c43-ec8152397e5f


<br />
<br />

<p align="center">
<ins>Utilize KQL to generate Security Logs in Sentinel:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/ca5e63ae-7aed-4b17-82a6-4eef47db0284


<br />
<br />

<p align="center">
<ins>Check security logs in the remote machine to verify a successful logon:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/20ab1ef0-d3cd-48f9-8c43-ec8152397e5f


<br />
<br />

<p align="center">
<ins>Utilize KQL to generate Security Logs in Sentinel:</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/ca5e63ae-7aed-4b17-82a6-4eef47db0284

<br />
<br />

<p align="center">
<ins> Change local Policy in VM :</ins> <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/9d7d9ce8-7a17-4bfc-ad78-046964f7e529



