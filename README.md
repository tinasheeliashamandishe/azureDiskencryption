<h1>Encrypt a Data disk using Azure Disk encryption</h1>

<h2>Description</h2>
This lab will Encrypt a Data disk using Azure Disk encryption.<br />
This lab assumes that you have already created a Windows virtual machine server, and added a data disk to the machine.
<br />

<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Step 1</h4>
Create a Key Vault Service Resource<br/>
<img src="https://i.imgur.com/CrHpDgD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<h4>Step 2</h4> 
In the Key Vault Resource, Generate a new Key of 4096 bits.<br/>
<img src="https://i.imgur.com/EGsVYw3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
In the Key Vault Resource, edit the key-vault cryptographic operations.<br/>
<img src="https://i.imgur.com/d176GRZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
In the Key Vault Resource, edit the access configurations. Allow volume encryption.<br/>
<img src="https://i.imgur.com/izcrsAI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />


<h4>Step 4</h4> 
Go to your VM -->disks-->additional settings--> encryption settings and encrypt using key in the key vault.<br/>
<img src="https://i.imgur.com/UzM4cKA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

<h4>Step 5</h4> 
The new disk is now encrypted using Azure Disk Encryption<br/>
<img src="https://i.imgur.com/bUigUJg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
