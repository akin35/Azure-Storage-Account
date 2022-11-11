## Azure-Storage-Account

During this project below steps will be followed. 

1.	Provision the lab environment
2.	Create and configure Azure storage accounts
3.	Manage blob storage
4.	Manage authentication and authorization for Azure Storage
5.	Create and configure an Azure Files shares
6.	Manage network access for Azure Storage 


## Solution:

### 1.	Provision the lab environment
* As a lab environment in the first step Azure VM will deploy.
* Before creating VM we will create a storage account named cloudshellakin123
* First rg0 is created on the eastus (picture1)
* And then vm0 with subnet0 and vnet0 (picture2)

### 2.	Create and configure Azure storage accounts
* In this step we will create a storage account in the rg1 from the Azure portal.
* Storage account name is storageaccountakin104
* All settings will be selected as default.
* In the redundancy setting scope we will select the Blob access tier as cool and LRS (picture 3 and Picture 4)

### 3.	Manage blob storage
*	From the azure portal select storage account and then select containers on the left pane and create the name az104-07-container (picture 5)
*	After creating the container, we will add the licence (picture 6)

### 4.	Manage authentication and authorization for Azure Storage
*	Copy the blob url to IE and click enter, the result is on picture 7
*	After generating SAS with value date, try the above step again with the newly generated url (pictures 8-9)
*	As a next step we will assign a new role (Storage Blob Data Owner) for the container from IAM 
*	Setting configuration can be seen in pictures 10-13.

### 5.	Create and configure an Azure Files shares
*	From the azure portal left pane on the storage account page, select file shares and create new named az104-07-share (picture 14)
*	After creating click the file and connect it via VM with the PowerShell script. (picture 15-17)

### 6.	Manage network access for Azure Storage 
*	From the azure portal left pane on the storage account page, selectnetworking and enabled from selected virtual networks and IP address (select your client pip) (picture 18)
*	After managing PIP, from IE click previously used url for blob. You can see download file.

## THANKS




