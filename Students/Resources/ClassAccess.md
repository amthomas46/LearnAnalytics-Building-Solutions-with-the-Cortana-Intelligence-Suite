Gaining Access to the Windows Data Science Virtual Machine
2
=================================================================================
3
​
4
Discover how to provision the Windows Data Science Virtual Machine (DSVM), a custom virtual machine image pre-installed and configured with a host of popular tools commonly used for data science and machine learning. This tutorial will take you through deployment of a DSVM, at no charge and without a credit card, with access for 72 hours.
5
​
6
### Provisioning the DSVM
7
​
8
1.  In an InPrivate/Incognito browser, navigate to the Cortana Intelligence Gallery page for the [Windows Data Science Virtual Machine](https://gallery.cortanaintelligence.com/Tutorial/Windows-Data-Science-Virtual-Machine-2), read through what you are getting, and click **Deploy**.
9
​
10
2.  In the new window, under “Don’t have an Azure account or subscription?”,  select **Try It Free**.
11
​
12
    >   *Note: this is why it is important to be in an InPrivate or Incognito browsing session.*
13
​
14
3.  Once provisioned, you will see a window labeled “Your Free Trial account is ready.” Be sure to save your username (i.e. freetrialuser-xxxxxx@ciqstestdrive.onmicrosoft.com) and password in a safe location. This is how you will log into the DSVM and the Azure Portal.
15
​
16
4.  After you’ve documented your username and password, select **Sign In**. The Microsoft login window will open; log in with your trial credentials.
17
​
18
5.  You’ll be redirected to the standard CIQS page, where some additional information is gathered to deploy your DSVM. At the top of the page, you’ll see what Resource group name you have been given (usually a nine-digit string of random characters)
19
​
20
    >   *Note: for the 72-hour free trial, you are given the ability to create and consume most resources and capabilities, with the exception of Resource Groups. You are not able to provision additional Resource Groups. Everything you create will go into the given Resource Group.*
21
​
22
As there are usually many interdependent components in a solution, Azure Resource Manager enables you to group all Azure services in one solution into a [resource group](https://azure.microsoft.com/en-us/documentation/articles/resource-group-overview/#resource-groups) Each component created is called a resource. We want to use a common name for the services we are creating. The remainder of this document will use the assumption that the base service name is:
23
​
24
    freetrialuser[UI][N]
25
​
26
Where [UI] is the user’s initials and [N] is a random integer that you choose. Characters must be entered in lowercase. Several services, such as Azure Storage, require a unique name for the storage account across a region and hence this format should provide the user with a unique identifier. For example, Steven X. Smith might use a base service name of *freetrialusersxs01*.
27
​
28
Enter in the following information and hit **Next**:
29
​
30
    Username: freetrialuser[UI][N]
31
    Password: (password that meets the requirements)
32
    Name for the Data Science Virtual Machine: freetrial[UI][N]
33
    Size for the Data Science Virtual Machine: Standard_A4 (default)
34
​
35
6.  Once provisioning is complete (about 5-10 minutes), you will be able to access your VM with Remote Desktop or through the Azure Portal. You are also given some additional resources (copied below).
