# Implementing a SQL database inside Azure using the Azure Portal
![SQLIcon](img/sql-icon.png)


---------------------------------------------------------


## Requirements
- Microsoft Azure Account ( with funds or credits    )
- Microsoft Azure Suscription
- A web browser
- Access to internet

---------------------------------------------------------

## Instructions
#### 1. Login to the [Azure Portal](https://portal.azure.com/).
#### 2. Once you're on the portal's home page, you will see something like this:
![PortalImage](img/portal-main.png)
#### 3. Click on the Cloud Shell Icon at the top of the page.
![CloudShellIcon](img/cloud-shell-icon.png)
#### 4. If you haven't used Cloud Shell before, you will need to create a storage account. Just click *Create storage* to do so.
![CreateStorage](img/create-storage.png)
#### 5. Once the storage has been created, you will be able to use Cloud Shell.
![CloudShell](img/cloud-shell.png)
#### 6. We'll be using [this](https://github.com/josejesusguzman/acordeon-az900-innovaccion/blob/main/res/consultas-sql.md) repository for guidance. First, copy the following commands and paste them one by one inside your Azure Cloud Shell (this may take a while).
```Bash
git clone https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals dp-900
```
```Bash
cd dp-900/sql
```
```Bash
bash setup.sh
```
![BashCommands](img/bash-commands.png)
#### 7. Once the process has been completed, click on the searchbar at the top of the page and look for *Resource groups*, then click on it.
![Searchbar](img/searchbar.png)
#### 8. Inside your last resource group, a SQL server and a SQL database have been created, click on it and make sure they're inside (if they aren't, look inside other resource groups until you find them).
![CreatedResources](img/created-resources.png)
#### 9. Click on the SQL database (Inventory).
![SelectedDatabase](img/selected-database.png)
#### 10. Click on *Overview* and then *Set sever Firewall*.
![SetServerFirewall](img/set-server-firewall.png)
#### 11. In *Firewall Rules*, click on *Add your client IPv4 address*.
![AddIPv4](img/add-ip.png)
#### 12. Click *Save*.
![Save](img/save.png)
#### 13. Go back to your database and click *Query editor*.
![QueryEditor](img/query-editor.png)
#### 14. Login to your database using the following credentials:
> Login: sampleLogin
> Password: samplePassword123!
#### 15. You are now able to do SQL queries to the table. For example:
```SQL
SELECT * FROM Inventory;
```
![SelectQuery](img/query-1.png)
#### 16. You can also insert items into your tables.
```SQL
INSERT INTO Inventory (Id, Inventory.Name, Stock) values(17, 'Pineapple', 999);
```
![InsertQuery](img/query-2.png)


---------------------------------------------------------

## Congratulations ! You've just implement a SQL Database inside Microsoft Azure !
