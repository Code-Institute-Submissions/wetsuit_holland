# Wetsuit Holland
This is an e-commerce website for selling wetsuits. 
The users can search in multiple ways on the website.
It’s possible to create an account and it will be able to purchase a wetsuit.

# Deployed Site (link website)

# UX
## User Stories
Viewing and Navigation by Shopper
•	View a list of all the products
•	View individual product details
•	Quickly identify different type of products
•	See the total amount in my shopping bag
Registration and User Accounts by Site User
•	Easily register for an account
•	Receive an email confirmation after registering
•	Easily login or logout
•	Easily recover my password
•	Have a personalized user profile
Sorting and Searching by shopper
•	Sort the list of available products
•	Sort a specific category of products
•	Sort multiple categories of products simultaneously
•	Search for a product by name or description
•	Easily see what i’ve searched for and the number of results
Purchasing an Checkout by shopper
•	Easily select the quantity of a product when purchasing it
•	View items in my bag to be purchased
•	Adjust the quantity of individual items in my bag
•	Easily enter my payment information
•	View an order confirmation after checkout
•	Receive an email confirmation after checking out
Admin and Store Management by store owner
•	Add a new product
•	Edit a product
•	Delete a product

## Strategy: What do we want to get out of the site? What do our users want?
This website is designed so users can scroll through the products and sort them in several ways. By clicking on a product they can read the product details and add the product to their shopping cart. When a product is added, the user can click checkout to complete their order by filling in the form.
Every user has the option to register for an account and to login at their account.
On this website the admin has the option to use all the CRUD functions: Create, Read, Update and Delete.

## Scope: What features will the site need to include?
All the folders:
•	bag: for users to see what is in their bag
•	checkout: with all the information before and after placing the order
•	home: the landing page where users can select how to view the products
•	wetsuit_holland: the Python code for this website
•	media: the images used on the website
•	products: a page with all the products and to view each product with more details
•	profiles: personal information and order history of registered users
•	templates:
o	The Base Page: with the whole navbar
o	The Navbar Pages: for displaying the navbar depending on the screen size
o	The Toasts: the pop-ups with extra information
o	The Allauth Pages: for all logging options
•	static: the base static file
•	readme: all the extra files for the README  ??? of in MEDIA ????

## Structure: How will the pieces of the site fit together and behave?
•	Header:
•	Top-navbar onlarge devices: on the left the title, in the middle the searchbar and on the right the menu items: My Account & Bag
•	The My Account dropdown menu will change, depending on if the user is logged out, logged in or it’s the admin
•	The Shopping Cart will change, depending on if the Bag is empty or filled
•	Main-navbar on large devices: with the menu categories in dropdown menu
•	Navbar on small & medium devices: 
•	Icon with dropdown menu: home & categories, each category has it's own dropdown menu
•	My Account dropdown menu will change, depending on if the user is logged out, logged in or it’s the admin
•	Shopping Cart will change, depending on if the Bag is empty or filled
•	Bottom: message
•	Landing Page: text and button to go to all the products
•	Signup Page: form field with buttons
•	Login Page: form field with buttons and checkbox
•	Profile Page: form field with buttons + order history
•	Logout Page: buttons
•	Password Reset Page: form field with buttons
•	Add Product Page: form field
•	Edit Product Page: form field with checkbox
•	Products Page: all products
•	Product Page: product details
•	Bag Page: button + added product
•	Checkout Page: buttons
## Skeleton: What components will enable people to use the site?
Main Nav Menu:
•	All Products is a collapsible menu: by Price, by Rating, by Category & all Products
•	Fullsuitis a collapsible menu: Mystic, Neilpryde, Prolimit & all Fullsuit
•	Shortarm is a collapsible menu: Mystic, Neilpryde, Prolimit & all Shortarm
•	Shorty is a collapsible menu: Mystic, Neilpryde, Prolimit & all Shorty
Top Nav:
•	Title: link to homepage (large device) or Home: link to homepage (medium/small devices)
•	Searchbar: searches through all wetsuits
•	My Account icon with dropdown menu:
•	Logged out user: Register, Login
•	Logged in user: My Profile, Logout
•	Logged in admin: Product Management, My Profile, Logout
•	Bag icon link to bag page
Delivery banner: text info
Homepage: button with link to all products page
Signup: 
	- Form field: e-mail address, e-mail address confirmation, username, password, password confirmation
	- Buttons: back to login, sign up
Login: 
•	Form field with: e-mail address, password
•	Checkbox: remember me
•	Buttons:  home, sign in
 
Password Reset: 
	- Form field: e-mail address
	- Button:  back to login, reset my password
Logout buttons: cancel, sign out
Profile: 
	- Form field: phone number, street address 1, street address 2, town or city, country, state or locality, postal code, country dropdown menu (all the countries included)
	- Button: update information
	- Overview order history:
Add Product: 
	- Form field: category dropdown menu, sku, product name, product description, sizes dropdown menu, rating, image url
	- Button: select image, cancel, add product
Edit Product: form field, the same as add product. Extra option: checkbox: remove image
Confirm E-mail: Button with confirm
Toasts: to display messages as pop ups on every page using django messages module, with messages for most actions across the website.

## Surface: What will the finished product look like?
•	Font Family text font: 
•	Background color: white
•	Home Page background: full image
•	Color schema: 
Top-navbar:
	- Text color: black
	- Text color inside searchbar: light grey
	- Background color: white
	- Icons: black
Header top-navbar and main-navbar on medium and small devices:
	Text color: black
	Text color inside searchbar: light grey
	Background color: white
	Icons color: black
Main-navbar:
	Text color: black
	Text color inside searchbar: light grey
	Background color collapsible product menu: 
	Background color collapsible Search and My Account icons: white
	Icons color: black
	Shopping Cart Icon when filled: 
Delivery banner: 
	- Text color: white
	- Background color:black
Home Page:
	Full page image
	Button: black, white text
	Button hover over: 
Sign Up Page:
	Background: white
	Title: dark grey
	Form: black borders, light grey text
	Button 1: white with black border, black text
	Button 2: black, white text
Login Page:
	Background: white
	Title:
	Form: white with black borders, light grey text
	Checkbox: unchecked
	Button 1: white with black border, black text
	Button 2: black, white text
Profile Page:
	Background: white
	Title: 
	Form: white with black borders, light grey text
	Button: black, white text
Logout Page:
	Background: white
	Title & text: dark grey
	Button 1: white with black border, black text
	Button 2: black, white text
Password Reset Page:
	Background: white
	Title & text: dark grey
	Form: white with black borders, light grey text
	Button 1: white with black border, black text
	Button 2: black, white text
Bag Page:
	Background: white
	Title & text: dark grey
	Button: black, white text
Add Product Page:
	Background: white
	Form: white with black borders, light grey text
	Button 1: black, white text
	Button 2: white with black border, black text
	Button 3: black, white text
Edit Product Page:
	Background: white
	Form: white with black borders, light grey text
	Checkbox: red, unchecked
	Button 1: black, white text
	Button 2: white with black border, black text
	Button 3: black, white text
Products Page:
	Background: white
	Images: black border
	Sort menu: white with black border, grey text
	Back to top icon: white with black border and arrow
	Product: image, dark grey price/title/tag/rating
	Light grey horizontal border between the products
Product Detail Page:
	Background: white
	Image: aligned whole left site on larger devices, aligned on top on smaller devices
	Title/price/tag/rating/product information: dark grey
	Quantity: left the minus icon, middle the quantity, right the plus icon
	Button 1: white with black border, black text
	Button 2: black, white text
Checkout Page:
	Background: white
	Form: white with black borders, light grey text
	Button 1: white with black border, black text
	Button 2: black, white text
	Order Summary with the products added to the bag:
•	Product Image
•	Product text: dark grey
•	Product value: black
Checkout Success Page
	Background: white
	Title & text: dark grey
	Button: black, white text
Confirm Email Page:
	Background: white
	Title & text: dark grey
	Button: black, white text

## Mockups
The following wireframes were created using Balsamiq to design the website layout options:
# Features
## Features left to implement
# Technologies
•	HTML5 was used as the main language for the templates
•	CSS was used for styling the webpage
•	JavaScript was used for some front end functionality
•	Python3 was used for backend data manipulation
•	Github was used for version control
•	Gitpod to build the website
•	Django was used as as a python based web framework
•	Django Allauth for the authentication system
•	Django Countries which was used for the country field for user to be able to select the country they are from
•	Django Crispy Forms to helps to manage the forms and able adjust forms properties in the backend
•	Gunicorn (‘Green Unicorn’) is a pure-Python WSGI server for UNIX
•	Pillow to be able to use the image field for the products on the site
•	Stripe to set up the payment methods for the site as customer can pay by card
•	Bootstrap for responsive simplistic layouts
•	JQuery for the JavaScript in the website
•	Font Awesome to add the icons used in the site
•	Amazon AWS for storing media and static files for use on my Heroku site
•	Autopep8 to tidy up my python code
•	SQLite 3 for the database which stores the information from my site e.g. products, users
•	W3C Markup was used this to check my HTML for errors and typos
•	W3C CSS was used to check the validity of my CSS
•	Google Chrome Developer Tools for testing different device sizes
•	Fontawesome was used for some icons on the website
# Deployment xxxx
# Credits
## Content
•	Plantsome for the product info in the plant section
•	The rest is made up by myself
## Media
•	Pixabay for some free images
•	Unsplash for some free images
•	Fontawesome for some free icons
•	Garyshood to resize the images
## Acknowledgements
•	Code Institute Course
•	YouTube
•	Slack Community
 
