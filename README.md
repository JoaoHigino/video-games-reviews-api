# video-games-reviews-api

## Introduction

The Video Games Reviews is a community site for game lovers. Users can post their reviews to the community, follow other users, like posts, favorite posts, comment on posts, and contact the admin. 

This repository holds the Django Rest Framework (DRF) API database for the ReactJS frontend part of the project. 

- [Deployed Front End Site](https://video-games-reviews.herokuapp.com)

- [Repository for Front End Site](https://github.com/JoaoHigino/video-games-reviews)

- [Deployed API Site](https://video-games-reviews-api.herokuapp.com)

- [Repository for API Site](https://github.com/JoaoHigino/video-games-reviews-api)


***
## Database

- The following models were created to represent the database model structure of the application:

![database](/docs/readme/database-schema.png)

***
## Validator Testing

All python files passed through the PEP8 validator with no issues

Contacts:

- [PP8 Contacts](/docs/test/contactmodels.png) - Models

- [PP8 Contacts](/docs/test/contactserializer.png) - Serializer

- [PP8 Contacts](/docs/test/contactsviews.png) - Views

Likes:

- [PP8 Likes](/docs/test/likesmodels.png) - Models

- [PP8 Likes](/docs/test/likesserializer.png) - Serializer

- [PP8 Likes](/docs/test/likesviews.png) - Views

Profiles:

- [PP8 Profiles](/docs/test/profilesodels.png) - Models

- [PP8 Profiles](/docs/test/postsserialzer.png) - Serializer

- [PP8 Profiles](/docs/test/profilesviews.png) - Views

Favourites:

- [PP8 Favourites](/docs/test/favouritesmodels.png) - Models

- [PP8 Favourites](/docs/test/favouritesserializer.png) - Serializer

- [PP8 Favourites](/docs/test/favouritesviews.png) - Views

Contact:

- [PP8 Contact](/docs/test/contactmodels.png) - Models

- [PP8 Contact](/docs/test/contactserializer.png) - Serializer

- [PP8 Contact](/docs/test/contactsviews.png) - Views

Posts:

- [PP8 Posts](/docs/test/postsmodels.png) - Models

- [PP8 Posts](/docs/test/postsserialzer.png) - Serializer

- [PP8 Posts](/docs/test/postsviews.png) - Views

***
## Testing

Backend Manual Testing


|Area|Test|Result|
|---|---|----|
|Deployed site|Home shows message and no errors|PASS|
||/profiles/ shows all profiles|PASS|
||/profiles/:id shows single profile|PASS|
||/posts/ shows all posts|PASS|
||/posts/:id shows single post|PASS|
||/comments/shows all comments|PASS|
||/comments/:id shows single comment|PASS|
||/admin/ allows superuser to login|PASS|
||/admin/ basic admin view and functions|PASS|
|Dev site|/posts/ show pagination|PASS|
||/comments/ show pagination|PASS|
||/profiles/ show pagination|PASS|
||/posts/ show text search by user__username|PASS|
||/admin/ shows login for Superuser and then loads admin panel|PASS|


### Manual testing of user stories

- As an admin, I want to be able to create, edit and delete the users, posts, comments and likes, so that I can have a control over the content of the application and remove any potential inappropriate content

**Test** | **Action** | **Expected Result** | **Actual Result**
-------- | ------------------- | ------------------- | -----------------
User | Create, update & delete user | A user can be created, edited or deleted | Works as expected
User | Change permissions | User permissions can be updated | Works as expected
Profile | Create, update & delete | User profile can be created, edited or deleted | Works as expected
Post | Create, update & delete | A post can be created, edited or deleted | Works as expected
Comment | Create, update & delete | A comment can be created, edited or deleted | Works as expected
Like | Create & delete | A like can be created or deleted (like / unlike post) | Works as expected
Follower | Create & delete | Follow or unfollow user | Works as expected

***
## Bugs

### Unfixed

None identified

***

## Technologies Used

### Languages and Frameworks Used

- [Python](https://www.python.org/)
- [Django](https://pypi.org/project/Django/3.2.14/)
- [Django-REST-framework](https://www.django-rest-framework.org/) - Toolkit for building web API's with Django.

### Python Modules Used

- Built-in Packages/Modules
  - [os](https://docs.python.org/3/library/os.html) - This module provides a portable way of using operating system dependent functionality.

### Packages Used

- External Python Packages
  - [cloudinary](https://pypi.org/project/cloudinary/) - Cloudinary intergration.
  - [django-cloudinary-storage](https://pypi.org/project/django-cloudinary-storage/) - Cloudinary intergration.
  - [dj-database-url](https://pypi.org/project/dj-database-url/) - Allows the use of 'DATABASE_URL' environmental variable in the Django project settings file to connect to a PostgreSQL database.
  - [django-allauth](https://pypi.org/project/django-allauth/) - Set of Django application used for account registration, management and authentication.
  - [dj-rest-auth](https://pypi.org/project/dj-rest-auth/) - API endpoints for handling authentication in Django Rest Framework.
  - [django-filter](https://pypi.org/project/django-filter/) - Application that allows dynamic QuerySet filtering from URL parameters.
  - [djangorestframework-simplejwt](https://pypi.org/project/djangorestframework-simplejwt/) - JSON Web Token authentication backend for the Django REST Framework.
  - [django-cors-headers](https://pypi.org/project/django-cors-headers/) - Django App that adds CORS headers to responses.
  - [gunicorn](https://pypi.org/project/gunicorn/) - Python WSGI HTTP Server.
  - [Pillow](https://pypi.org/project/Pillow/) - Fork of PIL, the Python Imaging Library which provides image processing capabilities.
  - [psycopg2](https://pypi.org/project/psycopg2) - Python PostgreSQL database adapter.


### Programs and Tools Used

- [drawSQL](https://drawsql.app/) - Create Database Schema/ERD
- [GitPod](https://www.gitpod.io/)
- [GitHub](https://github.com/)

<hr>

## Deployment

### Forking the GitHub Repository

By forking the GitHub Repository we make a copy of the original repository on
our GitHub account to view and/or make changes without affecting the original
repository by using the following steps...

1. Log in to GitHub and locate the [GitHub
   Repository](https://github.com/JoaoHigino/video-games-reviews-api)
1. At the top of the Repository (not top of page) just above the "Settings"
   Button on the menu, locate the "Fork" Button.
1. Click the button (not the number to the right) and you should now have a copy
   of the original repository in your GitHub account.

### Making a Local Clone

**NOTE**: It is a requirement of the project that you have Python version 3.8 or higher installed locally.

1. Log in to GitHub and locate the [GitHub Repository](https://github.com/JoaoHigino/video-games-reviews-api).
1. Under the repository name, click "Code".
1. To clone the repository using HTTPS, under "HTTPS", copy the link.
1. Open your local terminal with git installed
1. Change the current working directory to the location where you want the cloned directory to be created.
1. Type `git clone`, and then paste the URL you copied in Step 3.

    ```console
    ~$ git clone https://github.com/JoaoHigino/video-games-reviews-api
    ```

1. Press Enter. Your local clone will be created.

    ```console
    $ git clone https://github.com/JoaoHigino/video-games-reviews-api
    > Cloning into `test-dir`...
    > remote: Counting objects: 10, done.
    > remote: Compressing objects: 100% (8/8), done.
    > remove: Total 10 (delta 1), reused 10 (delta 1)
    > Unpacking objects: 100% (10/10), done.
    ```

    [Click here](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-a-repository-to-github-desktop) for a more detailed explanation of the process above with pictures.

1. Change the current working directory to the cloned project folder (this will be a child directory in the location you cloned the project).

1. It is recommended to use a virtual environment during development ([learn more about virtual environments](https://realpython.com/python-virtual-environments-a-primer/)). If you would prefer not to use one please skip the following steps:
    1. Create a virtual environment in the projects working directory by entering the following command in the same terminal window used for the steps above `python3 -m venv .venv`.
    1. Before use, the virtual environment will need to be activated using the command `source .venv/bin/activate` in the same terminal window used previously.
1. Packages required by the project can now using the command `pip install -r requirements.txt`
1. In the cloned directory, rename the file `.env-example` to `.env` and populate it with the information required.
1. Make Django migrations using the command `./manage.py migrate`.

### Deploying with Heroku

**NOTE**: It is a prerequisite of deployment to Heroku that you already have access to the following:

- A Cloudinary account, create one for free at [https://cloudinary.com](https://cloudinary.com).

**NOTE**: It is assumed you have followed all deployment instructions listed in this readme starting with the section titled 'Forking the GitHub Repository'.

1. Log in to [Heroku](https://www.heroku.com/) and if not taken there automatically, navigate to your personal app dashboard.
1. At the top of the page locate the 'New' drop down, click it and then select 'Create new app'.
1. Give your application a unique name, select a region appropriate to your location and click the 'Create app' button.
1. Your app should now be created, so from the menu towards the top of the page select the 'Resources' section.
1. Search for 'Heroku Postgres' under the Add-ons section and add it.
1. From the menu towards the top of the page select the 'Settings' section and lick 'Reveal Config Vars' in the Config vars section. Enter the following key / value pairings:
    1. Key as `ALLOWED_HOSTS` and the value as the name of you project with '.herokuapp.com' appended to the end e.g.  `example-app.herokuapp.com`. Click the Add button.
    1. Key as `CLOUDINARY_URL` and the value as your cloudinary API Environment variable e.g. `cloudinary://**************:**************@*********`. Click the Add button.
    1. Key as `SECRET_KEY` and the value as a complex string which will be used to provide cryptographic signing. The use of a secret key generator is recommended such as [https://djecrety.ir](https://djecrety.ir/). Click the Add button.
    1. Ensure the key `DATABASE_URL` is already populated. This should have been created automatically by Heroku.
    1. The `DATABASE_URL` should be copied into your local `.env`, created during the cloning process.
    1. To make authenticated requests to this API (e.g. from a fontend application) you are required to add the key `CLIENT_ORIGIN` with the value set as the URL you will be sending the authentication request from.
    1. Additionally, a `CLIENT_ORIGIN_DEV` key can be set with the value of a development server (IP or URL) for use during local development.
1. Open the `.env` file in the project directory and delete the key / value pair `DEV_ENVIRONMENT_DATABASE = True` before saving the file. This can be added back after the next step to ensure local development changes will not alter the remote database.
1. Navigate to the 'Deploy' page using the menu towards the top of the page.
1. Select 'GitHub' from the 'Deployment method' section and you will be prompted to 'Connect to GitHub'.
1. Once connected to your GitHub account you will be able to search for your repository which contains the forked 'property-direct-backend' repository.
1. Once the repository is found click 'Connect'.
1. At the bottom of the page find the section named 'Manual deploy', select the 'main' branch in the drop down and click the 'Deploy' button.
1. Once deployment is complete, click the 'View' button to load the URL of the deployed application.

<hr>

***

## Credits

- Code Institute's Moments project was used to lay the foundations of this project and was adapted on to create a unique project. 

- To my amazing wife Sandra, my best friend, my mentor, and my safe haven, without her, all my dreams will be impossible to achieve. She is everything.

- To my two kids, Maria and Thomas, with them life is easy and light. They make me laugh and think that our future is bright.

- To my family and friends - for being a great support and providing a lot of the user testing for me, especially my friends from "Liga 7 BP" with their craziness helped me to clean my head.

- To my mentor Lauren-Nicole aka CluelessBiker for all her help, feedback, and patience. It's a main difference when your mentor cares about you.

- The Code Institute community on slack and my classmates its was a pleasure. 

***