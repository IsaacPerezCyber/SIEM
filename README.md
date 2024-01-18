<H1>Azure Cloud Detection Using Sentinel</H1>

<h2>Description</h2>

- Configure and Deploy Azure Resources

- Log Analytics Workspace
    
- Virtual Machines
    
- Azure Sentinel

- Implement Network and Virtual Machine Security Best Practices

- Utilize Data Connectors to bring data into Sentinel for Analysis

- Understand Windows Security Event logs

- Configure Windows Security Policies

- Utilize KQL (Kusto Query Language) to query Logs

- Write Custom Analytic Rules to detect Microsoft Security Events

- Utilize MITRE ATT&CK to map adversary tactics, techniques, detection, and mitigation procedures

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
It will take a moment and then you should see this: <br/>
<img src="https://i.imgur.com/kreBoa3.jpeg" height="" width="70%" />

<br />
<br />

<p align="center">
Enable Microsoft Defender for Cloud: <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/eec687bf-e220-46d9-bd54-4a539fa66e0a


<br />
<br />

<p align="center">
We want to configure Just in Time Policy: <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/a7bfa792-dc5c-415e-a851-ca2367a5f1ca

<br />
<br />


<p align="center">
Then we make sure to set our connection rule: <br/>
<img src="https://i.imgur.com/xsUmwFW.jpeg" height="" width="70%" />
<p align="center">
Confirm:<br/>
<img src="https://i.imgur.com/i2c66NJ.jpeg" height="" width="70%" />


<br />
<br />



<p align="center">
Create Microsoft Sentinel Workspace: <br/>



https://github.com/IsaacPerezCyber/SIEM/assets/67014769/fd9a699a-1eb8-4118-92d0-bb9514b397a6



<br />
<br />

<p align="center">
Configure data collection rule for log integration in Microsoft Sentinel:<br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/eb745ca2-7577-4f93-a906-1a961536bf4f

<br />
<br />

<p align="center">
We make sure to confirm the log connection: <br/>
<img src="https://i.imgur.com/QovmfgQ.png" height="51%" width="30%" />

<br />
<br />

<p align="center">
Now we RDP into the VM to generate traffic on the Sentinel Logs:<br/>
<img src="https://i.imgur.com/ttFTvOB.jpeg" height="" width="80%" />


<br />
<br />

<p align="center">
Check security logs in the remote machine to verify a successful logon: <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/20ab1ef0-d3cd-48f9-8c43-ec8152397e5f


<br />
<br />

<p align="center">
Utilize KQL to populate Security Logs in Sentinel: <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/ca5e63ae-7aed-4b17-82a6-4eef47db0284


<br />
<br />


<p align="center">
 Change local Policy in VM : <br/>

https://github.com/IsaacPerezCyber/SIEM/assets/67014769/9d7d9ce8-7a17-4bfc-ad78-046964f7e529



<br />
<br />

<p align="center">
 Create task schedule in vm to generate log traffic in Sentinel : <br/>
<img src="https://i.imgur.com/6qXCbXg.png"  width="70%" />


<br />
<br />

<p align="center">
 Lastly, we write some KQL logic to alert us of the Task Scheduler : <br/>



https://github.com/IsaacPerezCyber/SIEM/assets/67014769/57bf063c-a24b-43fe-8eed-1ff3f222faea

<br />
<br />


<p align="center">
We are now monitoring live alerts from the persistent "malicious task" : <br/>



https://github.com/IsaacPerezCyber/SIEM/assets/67014769/1f8c8191-1ef6-483e-ba87-63cff43cbcc6














