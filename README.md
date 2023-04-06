## Dockerizing Django App

This is a sample code for dockerizing your django application with Postgres. We'll add on Nginx and Gunicorn as well.

### Dependencies

Django Rest JWT is a Python Django based platform. 

- Django v3.2.6
- Docker v20.10.8
- Python v3.9.6

### Usage

Following are the required steps to use this platform.

- Clone the repo
- Update the `.env` file
- Build the image
```sh
$ docker-compose build
```
- Once the image is built, run the container
```sh
$ Once the image is built, run the container
```

### Bonus

If you want to ssh the caontainer you can use the `makefile`

```sh
$ make ssh
```
then you can use all the django commands.

To generate static files for Django Admin, use:

```sh
$ docker-compose -f docker-compose.prod.yml exec web python manage.py collectstatic --no-input --clear
```
