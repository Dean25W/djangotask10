# djangotask10

# MySite
## This is the first interactive website i have built

## The entire purpose (besides asssignment submission) was to demonstrate the effective use of CSS, HTML and Django 
## The use of Django also encompassed user authentication, registration, login and logout pages as well as utilizing the polls functions


# Installation Guide:

# Creating A Virtual Environment
## In addition to downloaing all the files, you will need to install a virtual environment in order to run this website properly
## Assuming that you have already installed Django and pip to your local computer, follow the below inputs in your command terminal to create the virtual environment 
1. Change your directory to the main file using cd
2. Input "python3 -m venv venv"
3. Input "source venv/bin/activate" for MacOS or the appropriate function on your OS
4. Input "pip install django"
5. Navigate to where the manage.py file is and input "python manage.py runserver"
6. You should now be given a web address that will enable you to access the website

# Creating a Docker Image
1. Create a new file called Dockerfile with no extention
2. Add the following to the file:
   FROM nginx
   COPY . /usr/share/nginx/html
3. In your command terminal run: docker build -t my-website ./
4. In your command terminal run: docker run -d -p 80:80 my-website
5. Create a new repository on Docker
6. In your command terminal run: docker tag my-website [user]/[repo] (where user is your username on Docker and repo is your link to the repository on Docker
7. In your command terminal run: docker login
8. In your command terminal run: docker push [user]/[repo]

# Usage
## If a user is not registered, you will be prompted to register using the page below via [http://127.0.0.1:8000/register/](http://127.0.0.1:8000/register/) (see screenshot below)
![image](https://github.com/Dean25W/djangotask10/assets/139820372/4dbdc67e-2714-4591-8c82-122f73fd8a5a)

## Once registered, you will be taken to the login page where you can use your credentials to login to the main site (see screenshot below)
![image](https://github.com/Dean25W/djangotask10/assets/139820372/51089cfa-8a43-4360-8b90-2766a3696813)



