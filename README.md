Restaurant Menu App
==
Restaurant Menu App is a web application that provides a list restaurants with various menu items belong to each restaurant as well as provides a user registration via Google Account and authentication systems. Registered user can create new restaurants as well as make modifications to menu items of the restaurants s/he created.

Files explanation
--
project.py -- Python modules used to achieve app's major functionalities including JSON API Endpoints.<br>
database_setup.py -- Database schema and setup for the app.<br>
restaurantmenuwithusers.db -- Database created for the app. <br>
lotsofmenuswithusers.py -- Helper code for making up some database information for testing purpose.<br>

Setting up
--
1. Run <strong>database_setup.py</strong> to set up database.<br>
If you need to make up some inforamtion in database for testing, you can then run <strong>lotsofmenuswithusers.py</strong>.
<br>
2. Run <strong>project.py</strong> to start localhost on port 5000.<br>
3. Open browser and enter http://0.0.0.0:5000/ to direct to home page.<br>

Instruction
--
1. Browse the restaurant menu. <br>
You can view each menu by clicking the restaurant name without login.<br>

2. Login/Logoff <br>
You can login via Google account to get access of creating, editing and deleting items or restaurants of your own. <br>
To login click "Login" on the top navigation bar. <br>
To logoff click "Logoff" on the top navigation bar. <br>

3. Create Restaurant<br>
You have the access to create your restaurants after login. Once the restaurant being created, only the creator have the right to edit or delete the restaurant. The creators name is displayed on the menu page.<br>

4. Edit/Delete Restaurant<br>
Browser to the menu page of a restaurant you created and want to edit or delete, click the edit or delete button below the restaurant name.<br>

5. Modify Menu<br>
Browser to the restaurant menu you created and want to modify.<br>
To create the menu item click Add Item button below the restaurant name.<br>
To edit a menu item click the Edit button below the item information.<br>
To delete a menu item click the Delete button below the item information.<br>

6. JSON API<br>
There are three JSON APIs provided:
<ul>
<li>list of restaurants<br> /restaurants/JSON</li>
<li>a full menu items of a resstaurant<br> /restaurants/restaurant_id/menu/JSON </li>
<li>a menuItem's detail <br> /restaurants/restaurant_id/menu/menu_id/JSON </li>
</ul>
