# Active-Directory-Infrastructure
In this lab we will be building the foundation for an Active Directory Infrastructure. By changing the settings of the DNS IP Addresses of our clients we can enable them to have the same access to our domain controller throughout the network.
* Before we start this lab it will be recommended that we use Microsoft Azure to complete the following steps, a free subscription is available inside the software. If you are looking to make a new account and need assistance you can refer to the link provided this will give you a step by step guide on creating your account. https://www.youtube.com/watch?v=2bQ6WiJ1ncA


  # Creating a Resource Group


![image](https://github.com/user-attachments/assets/a94cf0ba-7f8b-4b2d-9e2e-f4968e11a4de)



1. Now that you have a subscription we will begin by going to the resource group tab, fill out the information you can name the resource "Active Directory Lab" and also make sure the location chosen falls within a U.S Territory such as "East US 2" this will ensure an accurate connection when accessing the domain controller.



# Creating a Virtual Network & Subnet

![image](https://github.com/user-attachments/assets/cb5af29d-fa74-4fa5-93a8-d2b359b8a89b)

2. Next we will create a virtual network and subnet, go to your homescreen and look for the "virtual Network tab there you will place the resource group we created earlier in the "Active-Directory Lab" and the name of this virtual Network will now be "Active-Directory Vnet"



# Creating A Domain Controller in Azure

![image](https://github.com/user-attachments/assets/15540d89-f078-4d15-b221-872b0c334179)


3. Given enough time to load up your virtual network will be created, next we will create a virtual machine once youv'e entered the tab there are certain acttions that must be followed
   1. Name: "DC-1"
   2. Resource Group: "Active Directory Lab"
   3. Region: "Same Region as your Resource Group & Virtual Network"
   4. Image: Windows "Windows Server 22"
   5. Tab over to the Networking Tab
   6. The Virtual Network should fall under "Active-Directory Vnet"
   7. Review and create your Virtual Machine

 4. We will create another virtual machine and follow similar steps to the first one with minor changes
    1. Name: "Client 1"
    2. Resource Group: "Active Directory Lab"
    3. Region: Same Region as your Resource Group & Virtual Network"
    4. Image: "Windows 10 version pro"
    5. Username:Labuser
    6. Password:Cyberlab123!
    7. Tab over to the Networking Tab
    8. The virtual Network should fall under "Active Directory Vnet"
    9. Review and create your Virtual Machine
   
  # Changing the NIC of the Domain controller to static
  ![image](https://github.com/user-attachments/assets/39a2bfb3-631d-4425-b083-f11594016d44)

   5. Now the Domain controller NIC has to be changed to static to keep the IP addresses from changing constantly, we will do this by going imto the network settings of our DC-1 virtual machine and changing the IP adresses from it's current setting (dynamic) to static.

# Disabling the firewall in the Virtual Machine

![image](https://github.com/user-attachments/assets/4f54d052-8d26-4539-8fc9-0c73b5d5a40c)










































        











