
![azure web app](https://github.com/Skizfly/AzureAppService/assets/153954157/ead9bf92-5ee7-4b62-bfec-81940b3e213a)


<h1>Deploy Web Application to Azure Web App (Azure)</h1>
Welcome to my tutorial on deploying a web app to Azure. I will illustrate the process of getting your application up and running on the Azure platform using Visual Studio.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure 
- Visual Studio
- PowerShell

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>Advanced Deployment and Configuration Steps</h2>

- Create Web App in Azure
- Create Web app framework 
- Connect deployment source 
- Deploy created app to Azure
- Test web app url in Azure

<h2>Azure Configuration Steps</h2>

![image](https://github.com/Skizfly/AzureAppService/assets/153954157/5708955e-78a2-4122-8509-affbf07fc76c)
![image](https://github.com/Skizfly/AzureAppService/assets/153954157/125f333e-d04b-4171-8c27-87375e20c5e9)

<p>
</p>
<p>
Before embarking on the setup, it's prudent to initiate a resource group for meticulous organization. Once that's established, proceed to the quest for "app services" in your Azure environment.
</p>
<br />

![image](https://github.com/Skizfly/AzureAppService/assets/153954157/757cb988-1f6d-4c85-86b0-bd0e6aa11f90)
![image](https://github.com/Skizfly/AzureAppService/assets/153954157/42e75c20-af3f-4d43-acf2-9db274d9dc53)
![image](https://github.com/Skizfly/AzureAppService/assets/153954157/0c2fc232-7fdd-4cbb-a516-b29e46893ca2)


<p>
</p>
<p>
Upon reaching the "App Services" section, click on the "Create" button, then select "Web App" from the dropdown menu (take note of other options and choose accordingly for your project). Assign a distinctive name to your app and configure the settings as per your requirements. Once done, proceed by clicking on "Review" and then "Create." Now, patiently wait for the deployment to complete and watch for the confirmation message.
</p>
<br />

![Capture](https://github.com/Skizfly/configuring-AD/assets/153954157/d31420cd-66d0-4348-83b8-8a7f8cb92525)

<p>
</p>
<p>
Now, proceed with installing Active Directory on the domain controller VM. In Server Manager, select "Add Roles and Features" and proceed. Verify the private IP address of the domain controller VM. In the Server Roles tab, choose "Active Directory Domain Services," add features, then click "Next" and "Install." Subsequently, promote the server to a domain controller. In Server Manager, address the warning sign in the top right corner, select "Promote this server to a domain controller." Opt for "Add a new forest" and define a domain name (e.g., lyanceytest.com). Set a domain password and click "Next" on each screen before selecting "Install."
</p>
<br />

<h2>A crucial point to consider</h2>
Upon relogging into the domain controller VM via Remote Desktop Connection, ensure logging in within the context of the domain. Input the domain path followed by the username, like mydomain.com\labuser. For instance, in my scenario, it is lyanceytest.com\labuser. With Active Directory installed, future configurations can be applied in subsequent labs, and the client VM will seamlessly join the created domain.
