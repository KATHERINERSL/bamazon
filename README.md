# bamazon

A mock storefront with departments and products. Customers, managers, and supervisors are able to use this app.

Motivation
A Node app for customers to view items and place orders, for managers to perform inventory control and add new products, and for supervisors to track department profitability and add new departments.

## Tech/framework used

#Built with:

- Node.js
- Javascript
- MySQL
- inquirer
- console.table
- Features
- Inquirer provides an easy to use UI with prompts asking the user what they would like to do.
- Customers may purchase products from the available products in the database.
- Managers have the ability to add inventory and new products to the databse.
- Supervisors have the ability to view profit data by department and add new departments.
- Console table organizes product, inventory, and department data in a concise manner within the CLI.
- User input validation is present to ensure that customers cannot purchase more inventory than Bamazon has in stock, managers don't add products with no inventory, and supervisors - - - cannot add departments that already exist.
- Installation
- Install Node js

Clone the Bamazon repository to your machine

Open CLI, navigate to the cloned repository, and run the following to install the npm package dependencies


  ``` npm install ```


Open MySQL Workbench, SQL Pro, or your preferred database management app. Open the "bamazon.sql" script from the cloned repo, and run it to set up the database and base product/department data.

Next, within the cloned repo, you'll need to create a pw.js file with the following code, and add your password to access your root server to that file. This file is a dependency for the app. If you do not require a password to access your root, simply leave the pw property as an empty string.

## var pwd = {
  ``` pw: "YOUR PASSWORD HERE" ```
``` } ```
	
``` module.exports = pwd; ```

## You're ready to go!

### How to use?

#### Customers

1. Run the following in your CLI while inside your cloned repo directory


  ```  node bamazonCustomer.js ```


2. Select from the resulting screen whether you would like to view items or leave.

3. If you select view items, input and enter the item id that you would like to purchase.

4. Input and enter the quantity that you would like to buy

5. If you would like to buy another item, repeat

6. If you would like to leave, click exit


- [View Products For Sale and Purchase](https://github.com/KATHERINERSL/bamazon/blob/master/images/customer_viewsales.PNG)


### Managers

1. Run the following in your CLI while inside your cloned repo directory


  ``` node bamazonManager.js ```


2. Select from the resulting screen whether you would like to view products for sale, view low inventory, add to inventory, add new product, or exit.

3. If you select add to inventory, follow the prompts for item id to increase inventory on and quantity to increase inventory

4. If you select add new product, follow the prompts for item name, department, price, and quantity in stock

5. When you are ready to leave, click exit

- [View Products For Inventory](https://github.com/KATHERINERSL/bamazon/blob/master/images/MGR_View.PNG)

- [Add Products For Inventory](https://github.com/KATHERINERSL/bamazon/blob/master/images/MGR_addnew.PNG)

- [View low Inventory](https://github.com/KATHERINERSL/bamazon/blob/master/images/MGR_Lowinventory.PNG)

- [Increase Inventory](https://github.com/KATHERINERSL/bamazon/blob/master/images/MGR_Addinventory.PNG)

### Supervisors

Run the following in your CLI while inside your cloned repo directory


  ``` node bamazonSupervisor.js ```


1. Select from the resulting screen whether you would like to view product sales by department, create a new department, or exit.

2. If you select create new department, follow the prompts for department name and overhead costs

3. When you are ready to leave, click exit

- [Supervisor View](https://github.com/KATHERINERSL/bamazon/blob/master/images/Supervisor_View.PNG)

- [New Department](https://github.com/KATHERINERSL/bamazon/blob/master/images/Supervisor_Newdepartment.PNG)





