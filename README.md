# Event Hive
## Installation

 - Clone or [download](https://github.com/ArthurAugustinho/Event-Hive/archive/refs/heads/main.zip) this repository;

 - Change directory to the projects folder and create a virtual environment;
  - On `\Event-Hive-repo`
    - `python -m venv venv_event_hive`
    - Activate the venv
      - `.\venv_event_hive\Scripts\activate`

- Install the dependencies;
  - On `\Event-Hive-repo`
    - `pip install -r .\requirements.txt`
    - 'python.exe -m pip install --upgrade pip'

- Run initial management commands

  - On `\Event-Hive-repo`
    - Create the database Migrations
      - `python .\manage.py makemigrations` 
    - Run the Migrations
      - `python .\manage.py migrate`
    - Collect Static Files
      - `python .\manage.py collectstatic --noinput`
    - Load the theme
      - `python .\manage.py loaddata`

- Create a Super User for testing
  - On `\Event-Hive-repo`
    - ` python .\manage.py createsuperuser` 

- Run the project
  - On `\Event-Hive-repo`
    - ` python .\manage.py runserver`
- Access the admin panel
  - Go to http://localhost:8000
    - Port may differ if you change it on "runserver" command.
