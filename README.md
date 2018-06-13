# Item Catalog Project
An Udacity Full Stack Web Developer Nanodegree project developed by Sai Narasimha.

## About
This application provides a list of players within various teams as well as provide a team registration and authentication system for players and teams. Registered players will have the ability to post, edit, and delete their own items.

### Features
- Proper authentication and authorisation check.
- Full CRUD support using SQLAlchemy and Flask.
- JSON endpoints.
- Implements oAuth using Google Sign-in API.

## Steps to run this project

1. Download and install Vagrant.

2. Download and install VirtualBox.

3. Clone or download the Vagrant VM configuration file.

4. Open the above directory and navigate to the `vagrant/` sub-directory.

5. Open terminal, and type

   ```bash
   vagrant up
   ```

   This will cause Vagrant to download the Ubuntu operating system and install it. This may take quite a while depending on how fast your Internet connection is.

6. After the above command succeeds, connect to the newly created VM by typing the following command:

   ```bash
   vagrant ssh
   ```

8. Type `cd /vagrant/` to navigate to the shared repository.

9. Download or clone this repository, and navigate to it.

11. Install or upgrade Flask:
    ```bash
    sudo python3 -m pip install --upgrade flask
    ```
12. Run the following command to set up the database:
    ```bash
    python3 database_setup.py
    ```
13. Run the following command to insert dummy values. **If you don't run this, the application will not run.**
    ```bash
    python3 fake_db_populator.py
    ```
14. Run this application:
    ```bash
    python3 app.py
    ```
15. Open `http://localhost:5000/` in your favourite Web browser, and enjoy.
