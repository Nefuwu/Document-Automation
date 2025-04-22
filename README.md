# Document-Automation
Welcome to the Enhanced Document Automation System! This powerful web-based tool allows you to upload scanned documents such as invoices, automatically extract key data using OCR and NLP technologies, and seamlessly integrate with any of your businesses like a financial software for efficient management of invoice records.


## Features

- Custom authentication with backend support
- Django templating for frontend pages
- Form handling and validation
- Custom filters for template rendering
- Admin interface
- Static file management

## Project Structure

- `main/`
  - `accounts/` – App containing views, models, forms, and templates
    - `templates/` – Django templates for HTML rendering
    - `migrations/` – Database migration files
    - `forms.py` – Form classes for user input
    - `models.py` – Data models
    - `views.py` – View functions and logic
  - `myproject/` – Django project configuration
    - `settings.py` – Main project settings
    - `urls.py` – URL routing
  - `static/` – Static assets (e.g. images, CSS)
  - `db.sqlite3` – SQLite database (for development use)
  - `manage.py` – Django CLI entry point
  - `requirements.txt` – Project dependencies


## Installation & Setup

Follow these steps to set up and run the project locally:

1. **Clone the repository**
 ```sh
 git clone https://github.com/Nefuwu/Document-Automation.git
 cd main
```
   
2. Create a virtual environment by running the following command:
```sh
python -m venv .venv
```

3. Activate the virtual environment:
On Windows, run:
```sh
source .venv/Scripts/activate
```
or
```sh
.venv/Scripts/activate
```
On macOS and Linux, run:
```sh 
source .venv/bin/activate
```

4. Install the required dependencies by running the following command:
```sh
pip install -r requirements.txt
```

If there's an error after installing the requirements.txt, try running this if you don't have the latest version of pip. Then install the requirements again.
```sh
python.exe -m pip install --upgrade pip
```

5. Apply database migrations
```sh
python manage.py migrate
```

6. Create an admin user
```sh
python manage.py createsuperuser
```

7. Run the development server
```sh
python manage.py runserver
```
