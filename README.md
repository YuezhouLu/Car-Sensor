# Car Sensor

![Screenshot](/screenshot.png)


## Project Overview
  To develop an application that provides a list of items within a variety of categories as well as provide a user registration and authentication system. Registered users will have the ability to post, edit and delete their own items.


## Why This Project?
  Modern web applications perform a variety of functions and provide amazing features and utilities to their users; but deep down, it’s really all just creating, reading, updating and deleting data. In this project, you’ll combine your knowledge of building dynamic websites with persistent data storage to create a web application that provides a compelling service to your users.


## Skills Honed
+ Developing a RESTful web application utilizing:
    1. Python
    2. Flask Framework
    3. HTML
    4. CSS
    5. OAuth 2.0
+ Implementing CRUD (create, read, update and delete) operations.
+ Implementing third-party OAuth authentication.


## Files in this Repo
  This project has one main Python module _**app.py**_ which runs the entire Flask application. A SQL database called _**mygarage.db**_ is created using the _**database_setup.py**_ module and you can populate the database with test data by running _**lotsofcars.py**_. All front-end HTML templates of this Flask application are stored in the _**templates**_ folder, and CSS file is stored in the _**static**_ directory.


## How to Run?
### Prerequisites and Dependencies:
* Terminal
* Git
* Python ~2.7
* Vagrant
* [Udacity Vagrant file](https://github.com/udacity/fullstack-nanodegree-vm)
* VirtualBox

### Setup the project:
1. Install [**Vagrant**](https://www.vagrantup.com/downloads.html) & [**VirtualBox**](https://www.virtualbox.org/wiki/Downloads).
2. Download or clone the Udacity [**fullstack-nanodegree-vm**](https://github.com/udacity/fullstack-nanodegree-vm) repository.
3. Download or clone this **Item-Catalog** repository.
4. Find the _catalog_ folder under the _vagrant_ directory, and replace it with the content of this **Item-Catalog** repository.

### Launch the project:
1. Launch the Vagrant VM.  
    ```$ vagrant up```
2. Login to Vagrant.  
    ```$ vagrant ssh```
3. Navigate to the catalog folder under vagrant directory.  
    ```$ cd /vagrant/catalog```
4. This App imports **requests** which is not on this VM, so run `$ sudo pip install request` to install **requests**. Also, install any other packages which will be used in the App but not included in this VM yet.  
    ```$ sudo pip install ...```
5. Initialize the database.  
    ```$ python database_setup.py```
6. Populate the database with some initial fake data.  
    ```$ python lotsofcars.py```
7. Fire up the application server.  
    ```$ python app.py```
8. Access and test the App by visiting **http://localhost:5000** on any browser you like.


## Public JSON Endpoints
#### The following JSON API Endpoints are open to the public:
>* Returns all makers' information in JSON format:  
    ```/garage/JSON```
>* Returns info of all models of a specific maker in JSON format:  
    ```/garage/<int:maker_id>/model/JSON```
>* Returns information about a specific model in JSON format:  
    ```/garage/<int:maker_id>/model/JSON```


## New Updates & Features
- _**updated on Oct 24, 2018:**_
    >- Created this README.md file.
    >- Saved the screenshot of the application.


## References
1. The [Restaurant Menu Project](https://github.com/YuezhouLu/OAuth2.0)
2. Other [Item Catalog Project](https://github.com/gmawji/item-catalog)