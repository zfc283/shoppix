## Description
Shoppix is a full-featured Django backend for modern e-commerce applications, delivering RESTful APIs for comprehensive product, category, and content management (including banners and featured items), as well as user profiles, authentication, and order processing

&nbsp;

## Screenshot
&nbsp;

<img src="https://zfc283-wiki.s3.ca-central-1.amazonaws.com/github-readme-images/Screenshot+(443).png" alt="Alt text" >

&nbsp;

## Setup
To get started, follow the following steps:
1. Install project dependencies (Python 3.6, virtualenv, MySQL8.0) on your local machine
2. Clone the repository to the local environment using: `git clone <repository-url>`
3. Create a virtual environment, copy `requirements.txt` to `path_to_virtual_environment/Scripts`, activate the virtual environment, and then run `pip install -r requirements.txt` to install the project dependencies
4. Open the project in PyCharm, set up the Python Interpreter in settings to use the `python.exe` executable from the created virtual environment. Then after PyCharm has finished loading the project, mark the `apps` and `extra_apps` folders as Sources Root 
5. Create a new database
6. Configure your database connection settings in `Shoppix/settings.py`
7. Navigate to the project root folder and issue the command `python manage.py migrate` from the command line to apply migrations to the database schemas
8. Run the `import_category_data.py` and `import_goods_data.py` scripts located in the `db_tools/data` folder in sequence to populate the database with data records
9. From the project root folder command line, issue the command `python manage.py runserver` to run the project, or alternatively, launch it from PyCharm by clicking the Run button in the top right corner
