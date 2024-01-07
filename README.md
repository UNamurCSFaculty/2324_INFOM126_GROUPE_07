# Django Polls App

This is a simple Django Polls app that allows users to create and participate in polls.

## Features

- Create new polls with multiple-choice questions
- Users can vote on existing polls
- View results of polls in real-time

## Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07.git
    ```

2. Navigate to the project directory:

    ```bash
    cd 2324_INFOM126_GROUPE_07
    ```

3. Set environment variables

    ```bash
    source env_example.sh
    ```
    - You can also specify your own values for the environment variables by creating either a `env_dev.sh` or a `env_prod.sh` file (those names are in the `.gitignore`)
### Using Docker (Recommended)

1. Fire up the container

    ```bash
    docker compose -f docker-compose.dev.yml up --build -d
    ```

2. Apply migrations:

    ```bash
    docker exec django_dev python manage.py migrate
    ```

3. Create a superuser (admin) account:

    ```bash
    docker exec -it django_dev python manage.py createsuperuser
    ```

4. Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser to access the app.

### Using virtualenv & pip

1. Create a Virtualenv
    - Windows
    ```bash
      pip install virtualenv
      virtualenv .venv
      .venv/Scripts/activate.bat
    ```

    - Linux
    ```bash
      sudo pip3 install virtualenv
      virtualenv .venv -p python3
      source .venv/bin/activate
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Apply migrations:

    ```bash
    python manage.py migrate
    ```

4. Create a superuser (admin) account:

    ```bash
    python manage.py createsuperuser
    ```

5. Run the development server:

    ```bash
    python manage.py runserver
    ```

6. Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser to access the app.

## Usage

1. Login to the admin interface using the superuser credentials:

    ```bash
    http://127.0.0.1:8000/admin/
    ```

2. Create new polls and questions.

3. Navigate to the polls section of the app:

    ```bash
    http://127.0.0.1:8000/polls/
    ```

4. Vote on existing polls and view the results.

## Contributing

Check out our [guide](docs/CONTRIBUTING.md) for new contributors to get started.
