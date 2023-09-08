# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
<p align="center">
<img src="https://github.com/Jacobvillagomez1/post-install-config/assets/143027686/e57ef384-fb94-4fe2-a701-ebc1ab6d2b5a"/>
</p>
<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://youtu.be/fX-EOyscj6w)

- ⬇️⬇️⬇️⬇️⬇️Use this link to download the files⬇️⬇️⬇️⬇️⬇️
- https://drive.google.com/drive/folders/1gX3eCEKAB4RzKLbkAimJi77gjwS_nxl7?usp=sharing

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- OsTicket 

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- HeidiSQL
- MySQL
- OsTicket
- PHP Manager
- php
- Rewrite
- VC_redist

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/fa537c14-03b8-4e30-9b39-8a87fa05dabf"/>
</p>
<p>
First go to Microsoft Azure and type Resource Group then click create Resource Group
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/4411c1f1-0cf9-4a78-aadc-3d27c6b34946"/>
</p>
<p>
Now type RG-osticket for the name of the Resource Group. Next for the region click US West US 3 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/eff6d1ee-3474-4ea3-b73a-87c97f082a6a"/>
</p>
<p>
Now go to the review and create tab and click the create button on the bottom left 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/df5e9844-91e1-440b-b3fe-fd29d9b5fa9e"/>
</p>
<p>
Now type Virtual Machines and click create azure virtual machine 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/cb8a5a02-b384-4980-aa1f-4b59802e6d30"/>
</p>
<p>
Now select the resource group we created RG-osticket then the virtual machine name type VM-osticket and the region select the same as the resource group US West US 3 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/74938101-497d-4fd2-98f2-a37d0c3593b9"/>
</p>
<p>
Now for the image select windows 10 pro version. For the size select standard Ec2 and the username type labuser and the password type a unique password remember to copy all this down on a notepad or physical paper
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/b50019f0-ddcf-4a12-919c-542c96d935e0"/>
</p>
<p>
Next click the licensing box and then click review and create 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e37cdcfd-b0c4-49ec-a404-f857fd297230"/>
</p>
<p>
Now go to the networking tab and make sure virtual network, subnet, and public ip all says (new)
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/aa85a26a-ba88-4299-92f6-5102aac9bdec"/>
</p>
<p>
Next create the virtual machine and you will see the deployment process start 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/d11832b6-49a0-49e6-805b-f72a9069c83b"/>
</p>
<p>
Now the process will be done when you see a green check mark 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e4a242f3-04f1-4f2b-8d95-2caa45bb360a"/>
</p>
<p>
Next go back to the virtual machine home page and click VM-osticket then copy the public IP address
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/54a098be-e769-43ab-a3b0-0d96aa70e7c7"/>
</p>
<p>
Next type Remote Desktop Connection in the search bar of your PC then click to open the app
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/27639ad0-fd28-4511-9e20-26f49b2e6c36"/>
</p>
<p>
Paste the public IP of VM-osticket into the computer section then click connect 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/16f1cecb-7064-45ad-98a2-f9efa9bb89c8"/>
</p>
<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/cbbc0261-d0f2-475f-9cf5-6579f2cca14b"/>
</p>
<p>
now for the user name type labuser and the password type the password you made for the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c14f377c-ff81-4314-98ce-a3cdbcd715aa"/>
</p>
<p>
Next click yes to connect to the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/b00ae585-36e3-49b2-ba7b-012404b2f796"/>
</p>
<p>
Now you will see the virtual machine log into labuser load
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/9ffead6c-4b08-444a-8223-8c2f5d16661d"/>
</p>
<p>
Now click no for all the following in the image above 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/081fb0bc-7143-403c-9b80-6cf81c7c2491"/>
</p>
<p>
Now once the networks tab shows on the right side of the screen then click yes 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/7626cf37-a8d9-4020-882f-0c15148e0d5f"/>
</p>
<p>
Next right click the windows icon on the bottom left then click run 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/595c1128-d938-4e92-a399-d86804ef641a"/>
</p>
<p>
Now type control type then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/82a026ed-526c-45f7-8562-9c7406d04d12"/>
</p>
<p>
Now click programs 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/5a0f17a5-dbcd-49f8-aabe-a84207a13387"/>
</p>
<p>
Click programs and features
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ea423df3-a563-4f17-b17a-8007de3e9c64"/>
</p>
<p>
Now click Internet Information Services
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/d42c75c7-4921-4219-aeda-c299198931b5"/>
</p>
<p>
Now click world wide web services 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c71c54ff-8fc8-43fc-9c27-d93263712547"/>
</p>
<p>
Next click application development features 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ecbffb91-0e4c-45fa-992b-c9fbd532e067"/>
</p>
<p>
Next click the box for CGI
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f114579a-ceb8-4ecb-8b48-656b1d63dcc8"/>
</p>
<p>
Next click Common HTTP Features 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f577be71-ef65-4554-b40f-0088df36f689"/>
</p>
<p>
Now in Common HTTP Features click the box for everything then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f951f632-2872-4816-b339-7586ea44d7e8"/>
</p>
<p>
Then you will see a loading screen process 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/d3c8f6d1-b2f1-40f0-bb90-fcf03e41ec72"/>
</p>
<p>
Now open up microsoft excel and click start without your data
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/175c71d1-f746-4507-adeb-946718c85528"/>
</p>
<p>
Now click continue without this data 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/4e728615-2d5f-4c21-b43b-c4d1cf9bbcb1"/>
</p>
<p>
Next click confirm and continue 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a5ea5ff4-09a3-4213-b9e3-d5d281f3623b"/>
</p>
<p>
Finally click continue and start browsing 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/9851b44c-23d1-4d32-a61b-6ce5ad7526c1"/>
</p>
<p>
Next once the process is complete click close 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/6a79a3e7-d690-4a16-9b19-cd313e78ed8e"/>
</p>
<p>
Now in order to see if the process worked type 127.0.0.1 in the search bar and you will see the same image above 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/7ede1ce6-e69f-4421-99f3-e81ddeb05f91"/>
</p>
<p>
Next open the link and download PHP Manager for IIS click the download symbol on the side
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/557bc0ab-6ed6-4b2c-947c-c445bd5f0b53"/>
</p>
<p>
Now open up file explorer and go to your downloads folder then double click PHP manager 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f716cf3e-09b0-4626-99df-38eaa1e3af29"/>
</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/282eeedf-144b-4e5a-8f3b-5e10c680f1c5"/>
</p>
<p>
Next click I agree and then next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/bf7f526b-81bf-4bb4-ad28-c7c21fac535a"/>
</p>
<p>
Finally click close 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/dd9df8e2-659b-4457-a1d1-00d6bc838fd0"/>
</p>
<p>
Next go back to the link and download Rewrite Module click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/69b4befa-4082-4076-99b6-fa5726f2be5b"/>
</p>
<p>
Go back to file explorer and double click rewrite 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/d8577920-628a-493c-bf85-6c23f01e8a48"/>
</p>
<p>
Click I accept then install 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/092f4b48-9225-4a7f-9674-aa9569bb6d04"/>
</p>
<p>
Now let the process start 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/46a693bc-84bb-4023-a4d4-ffa5ae957512"/>
</p>
<p>
Next click finish
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/437b01b3-cb18-4a5d-b77d-9a1b169d8dab"/>
</p>
<p>
Next go back to the link and download PHP 7.3.8 click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c10e3dc0-4e13-43b9-ade7-d569f3b56190"/>
</p>
<p>
Go back to file explorer and you will see the file in the download folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a02af26e-5491-4005-938e-ff743d86e07e"/>
</p>
<p>
Now click on Windows (C) 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/14176c62-b5c9-43c8-8bd4-4e9177aa22ef"/>
</p>
<p>
From here right click anywhere and click new then select folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/7889b411-2c14-4dc2-92b9-c6b6228adfb3"/>
</p>
<p>
Now name the folder PHP
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/de31d752-c9a0-48e5-a9c4-f0308f22d181"/>
</p>
<p>
Go back to the download folder and right click php folder then click Extract All
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1e3de15f-05df-40a2-94ef-90223a2dc1a1"/>
</p>
<p>
Now click browse 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/de6ff1d7-429c-4a19-8678-72315387fd0e"/>
</p>
<p>
Next go to Windows (C) then click the PHP folder we created 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/db4b6ead-5edc-47d6-9b8a-2e223f4a9178"/>
</p>
<p>
Now once you are in the folder click select folder on the bottom right 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/288c3d65-7bff-47c0-8161-1b50fe62a534"/>
</p>
<p>
Now click the extract button
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/912c3522-5954-42fa-a380-933cd7957a99"/>
</p>
<p>
Next you will see all the files load into the PHP folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/9668435c-d238-4608-8022-7020a6e8bf38"/>
</p>
<p>
Next go to the link and click the link to download VC RedistX86.exe click the download symbol
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/5da2381e-027b-41ee-9df3-cbd21331a21d"/>
</p>
<p>
Now go to file explorer and double click VC_redist 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/2b2a82b7-ea2b-49b5-80b7-dc333e7e2bc0"/>
</p>
<p>
Click Install 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/be911f23-5a1f-459b-bf54-5a251a45a236"/>
</p>
<p>
Now once the process is done click close 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e619f6d7-0ded-4bc0-a953-ff2bdf7e0c27"/>
</p>
<p>
Next click the link an download MySQL 5.5.62 then click the download symbol 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c76ee24a-f88b-444d-ba1b-d3783dc2d6d8"/>
</p>
<p>
Now go to file explorer and double click mysql to open the program 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/20c47cb8-c2f9-48eb-95d2-d7884a07d734"/>
</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/008e08c5-a0b1-48a1-a669-d23511da9b39"/>
</p>
<p>
Next click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ed8dad36-e031-417d-9b9f-3d2640d59f12"/>
</p>
<p>
Now click Typical 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/937d59b3-4945-40f8-8757-2c6edc041c51"/>
</p>
<p>
Next click install 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1f4fc9ed-d2f2-4445-b61d-b1ee1f4d6a3f"/>
</p>
<p>
Now click finish 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/cb13b58c-6c6f-46a1-bbf6-09986ded6e1f"/>
</p>
<p>
Now click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1926c0fc-b984-438d-b863-8d3d993ac0ea"/>
</p>
<p>
Now click Standard Configuration then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a5aaf679-e76d-4e4d-bf58-d9cef62cbce8"/>
</p>
<p>
Now click Install as Windows Service then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/8308594d-9b64-400e-8de3-e794ed296f70"/>
</p>
<p>
Now type the password. For this example I'm going to type Password1 then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/43cc6062-a91c-45b0-8a92-6a6a54352a95"/>
</p>
<p>
Next click execute to finish the process
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e3da9c2f-3f14-4be1-9257-7655551e44fa"/>
</p>
<p>
You will then see the process finish 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/cadedd65-6d83-4410-a35d-80498ddc9a08"/>
</p>
<p>
Now type IIS or Internet Information Services then right click then click run as administrator 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/5f0a0fe5-14b6-4fcb-be1a-de682dce0d72"/>
</p>
<p>
Now click PHP Manager 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/4a0bfe9a-840e-48fa-ac4e-428cb082281f"/>
</p>
<p>
Next click Register new PHP version 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ebbc52d3-3b98-4d04-923d-bb8db0565ef2"/>
</p>
<p>
Now you will see this tab, click the three dots on the right side  
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/37ab34e9-80f1-489a-9b61-f52032aed5b0"/>
</p>
<p>
Now go to Windows (C) then click the PHP folder we created earlier 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/2145448d-3c40-41be-b8e0-d148f17f4ab4"/>
</p>
<p>
Now click the PHP foler then click php-cgi 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/2088c3cf-6797-45f8-a674-e6378ce5abd5"/>
</p>
<p>
Now you will see the path before you on the white bar then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/20c27225-d41e-4637-8edd-27bc194c39e1"/>
</p>
<p>
Now you will see that the caution sign disappeared from PHP Setup
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/6640a965-fdfe-4a0f-b1e1-3d247d23993d"/>
</p>
<p>
Go back to Microsoft Azure and click VM-osticket then click restart. Then click yes to restart the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/3a46f250-37fd-4d70-847a-22b7f7b16f17"/>
</p>
<p>
Now you will see that the VM is loading 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c78817ef-dd63-4454-b60f-39eac21ff56e"/>
</p>
<p>
Now go to the link and download osTicket then click the download symbol
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/628b7a9f-2c18-4acd-a0d0-e4e556907578"/>
</p>
<p>
Next open file explorer and you will see osTicket was installed as a zip file 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/0fda9fa0-2436-496a-9c11-69cb9dacb6ee"/>
</p>
<p>
Next go to Windows (C)
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/45b9b90a-84c1-45aa-b7e6-2ea1c0aa785f"/>
</p>
<p>
Next click inetpub folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/bbf29450-52f0-41ff-ad80-53c9c17caf42"/>
</p>
<p>
Now click the wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/df9cc101-2472-40d4-be92-54ee43ef90c7"/>
</p>
<p>
Now you will be in the wwwroot folder and see the following 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/2393e12c-ada5-4532-8ed5-af6f456cad69"/>
</p>
<p>
Next go back to the osTicket folder and click the upload folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/8ab5c340-0c96-4c88-bc5b-8e407b26c4c4"/>
</p>
<p>
Now drag the upload file to the wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e498f010-8092-4e5b-9fe1-a223e392605f"/>
</p>
<p>
Once the files are done copying over rename the file osTicket in wwwroot folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1bdebc35-ffc8-421e-a1a5-f82d0750f6a2"/>
</p>
<p>
Next type IIS or Internet Information Services then right click and open as administrator
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/8f159bee-0b7b-4625-9a7f-f8987bdbea71"/>
</p>
<p>
Now click the VM-osticket and then click restart on the right side 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ac9a6e67-47a2-4e1c-b8d2-0774756155fc"/>
</p>
<p>
Next click the sites folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/b53533a6-5499-495b-9d12-2888c9fe441c"/>
</p>
<p>
Next click the osTicket folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/0b312203-94be-4dfc-b1f6-b8003c65afb8"/>
</p>
<p>
Now click Browse *80 (http) 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/075cdf14-74d8-48db-932f-ebcfb99cdce3"/>
</p>
<p>
You will see the page load with alot of green check and red checks 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/9e4cd293-049d-4e3e-bfc1-b3384f31798a"/>
</p>
<p>
Next go to PHP Manager 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/09fd821f-6935-4610-a48b-86d3e49b3528"/>
</p>
<p>
Next click enable or disable an extension 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/bbb4ad96-ae43-4098-97b8-0460b4258dea"/>
</p>
<p>
Now find php_imap.dll we can see its disbale then click, then go to the top right then click enable 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/d272733a-a8f5-42e6-a104-a8acf1d87e06"/>
</p>
<p>
Now find php_intl.dll then click, then go to the top right then click enable 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/76650fea-0640-49b0-a41a-e40fbf2d3456"/>
</p>
<p>
Now find php_opcache.dll then click, then go to the top right then click enable
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f56f70f5-6900-4801-aa07-578c9e2a9855"/>
</p>
<p>
Now go back to the osTicket home page 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/07f2bf28-3b75-4b93-9d9c-b93c420cb762"/>
</p>
<p>
Next click continue 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a2a60e2c-1ff6-4bcf-96ae-cc58edbae2ea"/>
</p>
<p>
Now go back to the osTicket folder from wwwroot
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/3ea95a96-51ad-4e58-b83a-b0efefa789bd"/>
</p>
<p>
Next click the include folder 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/42c79898-b086-4a31-9fb0-1fec407d6a2c"/>
</p>
<p>
Now click ost-sampleconfig.php
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/7fc88de0-5eca-4a5d-9256-4c6bc2407a9b"/>
</p>
<p>
Now rename the file to ost-config.php
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/811492d9-ef0b-47d5-b51f-e11fc80f25ab"/>
</p>
<p>
Next right click the file then go to properties 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/fa970fff-95f5-4221-b56c-94db11a0d440"/>
</p>
<p>
Now click the security tab 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a46381c5-d906-481f-bec0-f9cb3783d8ed"/>
</p>
<p>
Next click the advanced button
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/55a113f1-bffb-4338-9bc9-5621c7368e77"/>
</p>
<p>
Now click disable inheritance 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/cffb17c6-f381-4187-af58-93ae40460bf0"/>
</p>
<p>
Next click remove all inherited permission from this object 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/8ad6d188-2cbd-44fb-8509-fe4ba7176163"/>
</p>
<p>
Next click add 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/176efbeb-5fdc-4a70-9a44-1c9c59d0ac4e"/>
</p>
<p>
Next click select a principal
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/85fc3f75-b2ad-46d6-83a4-63d26dc9e2ce"/>
</p>
<p>
Now type everyone 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a857d05b-234a-475c-9f9b-55cfc4368e3c"/>
</p>
<p>
Now click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/4c34624d-f5e2-48df-8b73-e9fb157fafe2"/>
</p>
<p>
Now click all the permissions then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1c591885-b33f-484d-aafe-f2ac5f5768ce"/>
</p>
<p>
Now click apply 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/7be67c43-7a1e-4804-985d-a2c216d5c44b"/>
</p>
<p>
Next click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/3c17f685-1f6e-4e1b-9b23-8d4eab55626b"/>
</p>
<p>
Now click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/3998f1b6-1ca6-43c2-bc39-bc7b02703444"/>
</p>
<p>
Next go back to the OsTicket home page and click continue
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/0563e86f-5b37-4e20-97e5-28762d41a552"/>
</p>
<p>
For the helpdesk name type josh help desk, the deafult email type josh@help.com. Now for admin user the first name type josh then the last name type garcia. For email address type josh@gmail.com. For the username josh then type the password I will type Password1. 
</p>

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/f76320fc-4ab9-41f5-b3c4-a057330a89a1"/>
</p>
<p>
Now go to back to the link and download HeidiSQL then click the download symbol
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/28b301f0-e839-4cbd-8aea-f1d5bcdceb40"/>
</p>
<p>
Now go to file explorer and double click HediSQL
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c8d7d7ea-f9e5-483a-84ba-42fc48c34c14"/>
</p>
<p>
Next click I accept the agreement then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/4c09d5e1-a1ec-4ecd-b351-cff2644c9352"/>
</p>
<p>
Next click install
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/052ad3b3-ab82-4479-88bf-859a28d2f721"/>
</p>
<p>
You will see the process start 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/e52fd989-0735-449d-ac63-32d03400e29d"/>
</p>
<p>
Next click finish 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/93171893-f444-4e2c-a3ef-6ec6fa81f7ac"/>
</p>
<p>
Next click skip 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/02baf490-ba6b-4042-a825-0088e7c583ff"/>
</p>
<p>
Now type root
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/1c84cfb4-97d7-4014-a1ec-3dffb2c1c4c7"/>
</p>
<p>
Next for the password section type Password1 then click open
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/a4b4daff-d66e-4e86-b894-212d91c6f0f8"/>
</p>
<p>
Now you will see the unamed tab 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/ece476ab-ebc7-4c51-8fdb-6e20f89202e0"/>
</p>
<p>
Next type root for the MySQL Username then for the MySQL Password type Password1
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/5f2e5a35-ed90-497b-a8ff-d500552d2923"/>
</p>
<p>
Now right click Unamed then go to create new then click Database
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/27cf046b-9eb5-453b-8701-2b9be2d8b24e"/>
</p>
<p>
Next type osTicket then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/b8f9d0ff-d1d1-458b-8ba0-5fc79b270f6f"/>
</p>
<p>
Next type osTicket for MySQL Database
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/735b889b-91fb-4865-bc1e-d641db847f10"/>
</p>
<p>
Now you will see the process load 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c0f2ae4e-4f2a-4ac4-bbdb-de5a3f21ba22"/>
</p>
<p>
Next you will see the process finish and osTicket was installed
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/76cd532d-f6ff-4f51-bae1-ff8e87505bf3"/>
</p>
<p>
Next go to the osTicket folder and delete the setup folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/5ed0cb3e-3f8b-4fcf-84c4-be1930ca41ed"/>
</p>
<p>
Now click ost-config.php
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/be19e868-c931-4ca5-b3f7-fa3d257cf0c6"/>
</p>
<p>
Right click and go to properties 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/6db9f04f-224a-4c5f-9cd4-92a9c6638a20"/>
</p>
<p>
Next click advanced 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/92146206-b6cc-416b-af36-8120cef97380"/>
</p>
<p>
Now click permissions
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/06516cbe-e712-4a18-b380-d183d9363823"/>
</p>
<p>
Next click allow everyone then click edit 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/405cc032-a569-40d3-a20b-a56bf757217a"/>
</p>
<p>
Now uncheck full control, modify, and write then click ok  
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/c28422dc-faf8-40aa-9408-334738c1d909"/>
</p>
<p>
Now click apply
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/osticket-prereqs/assets/143027686/20df729d-6052-413c-ba38-c9048da1ca23"/>
</p>
<p>
Finally click ok then click the link to continue the Post-Installation Configuration https://github.com/Jacobvillagomez1/post-install-config
</p>
<br />
