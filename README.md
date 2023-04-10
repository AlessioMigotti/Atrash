# ATRASH

**ATRASH**  website is developed using Django Framework as part of Portfolio Project 3 for my Full Stack Software Development Bootcamp at WAES useing Code Institute.

The target audience for the website would be businesses or individuals who are interested in buying recycled materials. The website could provide information about the types of materials that are available for purchase, pricing, and delivery options. The target audience could include manufacturers, construction companies, and individuals who are interested in using recycled materials for DIY projects and institutions.

You can view the live site here: >>>>>>>>>>>>>>

![mockup]

## [Content](#content)
- [ATRASH - Introduction](#ATRASH---introduction)
  - [User Experience - UX](#user-experience---ux)
    - [Site Aims](#site-aims)
    - [Agile Methodology](#agile-methodology)
      - [User Stories](#user-stories)
      - [Tasks](#tasks)
  - [Design](#design)
    - [Colours](#colours)
    - [Typography](#typography)
    - [Imagery](#imagery)
    - [Wireframes](#wireframes)
  - [Database Diagram](#database-diagram)
  - [Features](#features)
    - [Home Page](#home-page)
      - [Navbar](#navbar)
      - [Hero Image](#hero-image)
      - [Destination Section](#destination-section)
      - [Footer](#footer)
    - [User Page](#user-page)
    - [Staff Page](#staff-page)
    - [About Page](#about-page)
    - [Login](#login)
    - [Logout](#logout)  
  - [Admin Panel/Superuser](#admin-panelsuperuser)
  - [Technologies Used](#technologies-used)
    - [Languages Used](#languages-used)
    - [Django Packages](#django-packages)
    - [Frameworks - Libraries - Programs Used](#frameworks---libraries---programs-used)
  - [Walktrough](#walktrough)
    - [Steps](#steps)
  - [Bugs](#bugs)
      - [Fixed Bugs](#fixed-bugs)
      - [Unfix Bugs](#unfix-bugs)
  - [Credits](#credits)
    - [Content](#content)
    - [Information Sources / Resources](#information-sources--resources)
  - [Acknowledgement](#acknowledgement)


  # User Experience - UX

## Site Aims
* Provide a convenient and affordable service for individuals and businesses to have their trash collected and disposed of responsibly.
* Reduce the amount of waste that ends up in landfills or pollutes the environment by recycling and repurposing collected materials.
* Educate the public about the importance of responsible waste management and the environmental impact of their consumption habits.
* Promote a circular economy by creating new products and materials from recycled waste, thereby reducing the need for virgin resources.
* Partner with local organizations and businesses to support sustainable development and community-building initiatives.

## Agile Methodology
The Agile Methodology was used to plan this project. This was implemented through Trello and the Project Board. Through the use of the Kanban board, the project was divided into a few different sections:

* Doing
* Code Review
* Testing
* Done

Please find my Kanban Board made with Trello  [here](https://trello.com/b/x9zPyGwh/kanban-template).


## User Personas generated on [userpersona.dev](https://userpersona.dev/):
* ![UP0](assets/img/user-persona.png)
* ![UP1](assets/img/user-persona%20(1).png)
* ![UP2](assets/img/user-persona%20(2).png)
* ![UP2](assets/img/user-persona%20(3).png)
* ![UP3](assets/img/user-persona%20(4).png)
* ![UP4](assets/img/user-persona%20(5).png)
* ![UP5](assets/img/user-persona%20(6).png)

## Tasks

The tasks for the website development process was closely followed as mentioned in Legion Script 'Building a Food Delivery App' walkthrough project. The task is about the developers step by step, preparing the app.
The tasks that I have followed during the development phase were carried out in this order.

**Before Project Inception**

- Create Repository in GitHub
- Use CI template 
- Create Project, User Stories and prepare Kanban Board

**Creation of Project in GitPod**

- Create the django project. Check details in [deployment-section](#deployment)
- Deploying app to Ngruk - Details in [deployment](#deployment) section
- Create Database Models
	- Set up models.py file in directory
- Build Admin site
- Set up Templates
	- Create base.html - Navbar and Footer content, which gets extended to all the other template files
	- Add responsiveness to navigation and footer
    - Create index.html, view and style
	- Set up template file features with views.py and urls.py
  - about.html (Description about Trash)
  - order_confirmation.html (to confirm order and pay)
  - menu.html (to search an item)
  - order_pay_confirmation.html (to confirm the payment) 
- Install Allauth for sign in, sign up and sign out templates with-  pip3 install django-allauth 
	- Install crispy-forms to add styles to Django account templates with-  pip3 install crispy-bootstrap4
- Intensive Manual Testing and Validation checks of each page and codes written
- Final Deployment steps

-----

[Back to top](#content)

## Design

### Colours

The colour scheme has considered based on easy accessibility for all and have been consistently maintained throughout the website. The colours were chose using [Coolors](https://coolors.co/). 

![Color Palette](assets/img/color_pallete.png)

### Imagery

All the imagery is related to the trash and website design. Images are static and took from google images. The imagery was uploaded by the author to the database.

### Wireframes

The wireframes for this projected were generated using [Figma](https://www.figma.com/?fuid=). 
- ![Wieframe for index](assets/img/Section%2038.png)
- ![Wieframe for Menu](assets/img/Section%2022.png)
- ![Wieframe for Shop](assets/img/Section%209.png)

----

## Database Diagram

ERDPlus was used to create a database schema to visualise the types of custom models the project requires. This schema was used as a guide to what needed to be added to each model. Below is the Database structure that this project is based on.

![ER Diagram](assets/img/ERD%20regular%20background.png)

[Back to top ⇧](#content)

# Features

## Home Page

At the very first glimpse, user can see a Navigation bar. Homepage provides the user with some quick information about the site and make use of all its features. User do not need to be registered to order. The responsive navigation bar is featured on all pages. 

![Homepage](assets/img/Screenshot%20(106).png)

----


## Navbar

- The navigation bar is present at the top of every page and navigates all links to the respective pages.
- The options to Register or Log in will be only for the staff once a user has logged in.
- The navbar is fully responsive.

![Navbar](assets/img/Screenshot%20(108).png)

## User Page

* This page will be only visible to the user. The user navigates to the order page. On this user page, the user can view the list of services, we ask the custumer deatails.

![order-page](assets/img/Screenshot%20(118).png) 

* When user clicks on the order, the following form will be displayed.

![Pay-page](assets/img/Screenshot%20(117).png)

Last the payment confirmation will be displayed.

![Payment-confirmation-page](assets/img/Screenshot%20(118).png)


## Staff Page

* This page will be only visible to the staff. The staff navigates to the login page. On this user page, the staff can login to see the orders, and the custumer deatails.

![Login-page](assets/img/Screenshot%20(111).png) 

* When staff clicks on the login, the list of orders will be displayed.

![Staff-page](assets/img/Screenshot%20(112).png)

* Staff clicks on the edit, and the list of orders can be set as delivered.

![Staff-page](assets/img/Screenshot%20(112).png)




## Footer

- On the website footer, users can see basic information such as copyright, and login for staff.

![Navbar](assets/img/Screenshot%20(120).png)

----

## About Page

- The About Page gives, users information about Coders Trash with a brief discription of the benefits.

![About Us](assets/img/Screenshot%20(122).png

----

## Admin Panel/Superuser

- Admin accesses the project via logging into Django admin panel with a superuser id and password. The page appears as shown ![here](assets/img/Screenshot%20(126).png).
- A superuser "admin" was created for this project to manage the admin panel.
- On the Admin Panel, as an admin I have full access to CRUD functionality so I can view, create, edit and delete the following ones:
  - Categorys
  - MenuItems
  - Order Models
- As admin I can also approve orders, approve deliveries and change the status and give other permissions to the staff.

### Admin Model Management

- On selecting Blog "Post", a list of blog posts is displayed with its title, slug, status, created_on and author name. Admin can select the post and edit or delete its data.
- When a blog post is submitted by a user, its status is set to Draft by default.
- When the status is set to Publish on Admin Approval, the post starts appearing in the website.

The admin site for post model appears as shown ![here](assets/img/Screenshot%20(127).png).

### Admin 'Menu Item' Model Management

- Upon selecting the "Menu Item" model, a list of items is displayed. Admin can select the item and edit or delete its data.
- When a order is submitted by a user, it requires approval from an admin in order to publish it's contents.

The admin site for 'Menu item' model appears as shown ![here](assets/img/Screenshot%20(128).png).
The admin site for 'Order' model appears as shown ![here](assets/img/Screenshot%20(130).png).

----

## Technologies Used

### Languages Used

* [HTML 5](https://en.wikipedia.org/wiki/HTML/)- Used to structure all the templates on the site
* [CSS 3](https://en.wikipedia.org/wiki/CSS)- to provide extra styling to the site
* [JavaScript](https://www.javascript.com/)- Minimum javascript was used to fade out alerts after a few seconds.
* [Python](https://www.python.org/)- To provide the functionality to the site. Packages used in the project can be found in requirements.txt

### Django Packages

* [Crispy_bootstrap](https://studygyaan.com/django/how-to-use-bootstrap-4-forms-with-django-crispy-forms)- As the server for Heroku.
* [Pillow](https://pypi.org/project/Pillow/)- Was used to host the static files and media for the site.
* [Allauth](https://django-allauth.readthedocs.io/en/latest/installation.html)- For authentication, registration, account management.
* [Crispy Forms](https://django-crispy-forms.readthedocs.io/en/latest/)- To style the forms.

### Frameworks - Libraries - Programs Used

* [Django](https://www.djangoproject.com/) was used as the framework for the back-end logic of the project. Django enables rapid and secure development.
* [Bootstrap](https://getbootstrap.com/)- Used to style the website, add responsiveness and interactivity.
* [Git](https://git-scm.com/)- Used for version control by utilizing the Gitpod terminal to commit to Git and push to GitHub.
* [GitHub](https://github.com/)- Used to store the project's code after being pushed from Git.
* [Figma](https://www.figma.com/login)- Used to make the project's wireframe.
* [Userpersona](https://userpersona.dev/)- Used to make the project's outline.
* [Youtube](https://youtube.com/)- Used to make the project's base.

-----

[Back to top ⇧](#content)

# Walktrough

## Steps
All the pages got a navbar and a footer.
* The index has an order burron that will bring you to the order page.
* The order page gives you the possibility to choose the service you prefere, you will have to provide thr deatails, that will be the address where the service will be executed. Press the button and it will take the user to the pay page.
* When you get to the pay page you'll see what you orxdered. I gave the option to to pay with paypal. When the payment is confirmed you'll see a payment confirmation page.

* From the nav bar you can access the about page that gives a overview of what we do.
* There is the option to see what the manu items are un the manu page, but you can't buy the product from that page.

* If you whant to access as a staff member you have to press the login link on the footer. This will require a password and when you login you will be able to see all the orders and the status.

* To login as the admin you need to access the django admin page, login and you will be able to modify the items on the website, the staff that can access.


| **Unfix Bug** |
| ----------- | 
| When ordering you can't pick more than one item, that could be considered a bug if you try to. But that's intentional, maybe i should've specified.
There where some problems with the resposivness of the background image on the index, that i didn't solve for a lack of time. The image had some issues and needed some work outside the development enviroment.


----




# Credits

## Code
- The basic set up of the website was done by strictly following the steps as described in Legion Script channel on Youtube
- Followed the project Django he performed:https://www.youtube.com/watch?v=gy8ypTWT4wY .

## Learning Resources
- Code Institutes Full Stack Framework Module, mainly the 'blog' walkthrough project.
- Legion Script Django project.
- [W3CSchool](https://www.w3schools.com/django/).

## Content and Media

Mostly images and post content are taken from the website https://www.google.com/.

----

## Acknowledgement

Special thanks to my mentor Richey Malhotra. I got to give credit to my fellow student Cedric Littman in a part this projects readme.

[Back to top](<#content>)
   








