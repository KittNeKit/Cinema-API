# CINEMA API
API service for cinema management written on DRF

## Features

- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

## Installing using GitHub:
Install PostgresSQL and create db

1. Clone the repository:

```bash
git clone https://github.com/your-username/cinema-API
```
2. Change to the project's directory:
```bash
cd Cinema-API
```
3. Сopy .env_sample file with your examples of env variables to your .env
file


4. Once you're in the desired directory, run the following command to create a virtual environment:
```bash
python -m venv venv
```
5. Activate the virtual environment:

On macOS and Linux:

```bash
source venv/bin/activate
```
On Windows:
```bash
venv\Scripts\activate
```

4. Install the dependencies

```bash
pip install -r requirements.txt
```

5. Set up the database:

Run the migrations

```bash
python manage.py migrate
```

6. Start the development server

```bash
python manage.py runserver
```

7. Access the website locally at http://localhost:8000.

## Run with Docker

Docker should be installed

```
docker-compose build
docker-compose up
```

## Getting access

- create user via /api/user/register/
- get access token via /api/user/token/