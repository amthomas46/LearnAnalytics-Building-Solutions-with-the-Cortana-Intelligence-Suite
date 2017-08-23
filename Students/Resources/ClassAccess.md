Gaining Access to the Windows Data Science Virtual Machine
=================================================================================

Discover how to provision the Windows Data Science Virtual Machine (DSVM), a custom virtual machine image pre-installed and configured with a host of popular tools commonly used for data science and machine learning. This tutorial will take you through deployment of a DSVM, at no charge and without a credit card, with access for 72 hours.

### Provisioning the DSVM

1.  In an InPrivate/Incognito browser, navigate to the Cortana Intelligence Gallery page for the [Windows Data Science Virtual Machine](https://gallery.cortanaintelligence.com/Tutorial/Windows-Data-Science-Virtual-Machine-2), read through what you are getting, and click **Deploy**.

2.  In the new window, under “Don’t have an Azure account or subscription?”,  select **Try It Free**.

    >   *Note: this is why it is important to be in an InPrivate or Incognito browsing session.*

3.  Once provisioned, you will see a window labeled “Your Free Trial account is ready.” Be sure to save your username (i.e. freetrialuser-xxxxxx@ciqstestdrive.onmicrosoft.com) and password in a safe location. This is how you will log into the DSVM and the Azure Portal.

4.  After you’ve documented your username and password, select **Sign In**. The Microsoft login window will open; log in with your trial credentials.

5.  You’ll be redirected to the standard CIQS page, where some additional information is gathered to deploy your DSVM. At the top of the page, you’ll see what Resource group name you have been given (usually a nine-digit string of random characters)

    >   *Note: for the 72-hour free trial, you are given the ability to create and consume most resources and capabilities, with the exception of Resource Groups. You are not able to provision additional Resource Groups. Everything you create will go into the given Resource Group.*

As there are usually many interdependent components in a solution, Azure Resource Manager enables you to group all Azure services in one solution into a [resource group](https://azure.microsoft.com/en-us/documentation/articles/resource-group-overview/#resource-groups) Each component created is called a resource. We want to use a common name for the services we are creating. The remainder of this document will use the assumption that the base service name is:

    freetrialuser[UI][N]

Where [UI] is the user’s initials and [N] is a random integer that you choose. Characters must be entered in lowercase. Several services, such as Azure Storage, require a unique name for the storage account across a region and hence this format should provide the user with a unique identifier. For example, Steven X. Smith might use a base service name of *freetrialusersxs01*.

Enter in the following information and hit **Next**:

    Username: freetrialuser[UI][N]
    Password: (password that meets the requirements)
    Name for the Data Science Virtual Machine: freetrial[UI][N]
    Size for the Data Science Virtual Machine: Standard_A4 (default)

6.  Once provisioning is complete (about 5-10 minutes), you will be able to access your VM with Remote Desktop or through the Azure Portal. You are also given some additional resources (copied below).

    -   [How-To Guide to the Data Science Virtual Machine](https://azure.microsoft.com/documentation/articles/machine-learning-data-science-vm-do-ten-things/)
    -   [Provision the Microsoft Data Science Virtual Machine Instructions (if using the Azure Portal)](https://azure.microsoft.com/en-us/documentation/articles/machine-learning-data-science-provision-vm/)
    -   [Pricing and alternative provisioning](https://azure.microsoft.com/en-us/marketplace/partners/microsoft-ads/standard-data-science-vm/)
    -   [Team Data Science Process Overview](https://azure.microsoft.com/en-us/documentation/learning-paths/data-science-process/)

### Accessing the DSVM

1.  Go to the [Azure Portal](https://portal.azure.com), and log in with your trial credentials. You’ll be directed to a “Welcome to Azure” tour, which you should go through ([video available here](https://channel9.msdn.com/Blogs/Azure/Get-Started-with-Azure-Portal?ocid=player)) if you are new to the Azure Portal.

2.  Once in the portal, you’ll see an empty dashboard. On the left menu, select **All resources**. You’ll see that along with your Virtual machine *freetrial[UI][N]*, you have a storage account, public IP address, network interface, and virtual network. Select your virtual machine.

    >   *Note: notice that the Start button is grayed out. This means your virtual machine is running. While you have 72 hours to use resources before they are all deleted, it is a good practice to make sure to Stop your virtual machine when it is not being used (in the “real world” you will be charged whenever it is running, even if you aren’t using it).*

3.  Select **Connect** to establish a remote connection to your DSVM. You will get a pop-up “What do you want to do with freetrial[UI][N].rdp?”, select **Save**, select **Open**, select **Connect**.

4.  You’ll get a Windows Security prompt for your credentials. Select **More choices**, select **Use a different account**. Enter the credentials to your DSVM, which are different than your Azure Portal credentials. When you get the warning, “Do you want to connect despite certificate errors?”, select **Yes**. You will then be connected to the DSVM.
