# Installations

How to work on django-python project?


Note: Virtual environment avoids python and django versions conflict for a project. Suppose you have a project which has to be cloned
      on your machine with its packages and dependencies given in requirements.txt file. And you have another version of django and python
      installed on your machine. Then two cases come into picture i.e. "without virtual environment" and "with virtual environment".

      1. Without virtual environment
         If you clone a project without setting up a virtual environment, your project may not work properly due to versions conflict between
         cloned project and what has already installed on your machine. So, this is bad idea

      2. With Virtual environment
         If you set up a virtual environment and clone a project for that environment, then packages and dependencies of the project will be
         confined to that environment only. And whatever dependencies and packages are listed in requirements.txt file will be installed and used.
         So no conflicts take place and your project runs as expected. So, this is good idea of setting up virtual environment first.       



To set up virtual environment, you need to install pip first

1. sudo apt-get install python3-pip


Then install virtualenv using pip3

2. sudo pip3 install virtualenv 


Now create a virtual environment

3. virtualenv ./environment_name
example: virtualenv ./env

Note: you can use any name insted of venv


You can also use a Python interpreter of your choice

virtualenv -p /usr/bin/python2.7 venv


Active your virtual environment with following command

4. source venv/bin/activate


To deactivate the virtual environment, use following command

5. deactivate


Note: If you have installed project in virtual environment, the project will run only after virtual environement is activated.
