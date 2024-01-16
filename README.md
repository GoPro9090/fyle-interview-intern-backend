# Fyle Backend Challenge

## Who is this for?

This challenge is meant for candidates who wish to intern at Fyle and work with our engineering team. You should be able to commit to at least 6 months of dedicated time for internship.

## Why work at Fyle?

Fyle is a fast-growing Expense Management SaaS product. We are ~40 strong engineering team at the moment. 

We are an extremely transparent organization. Check out our [careers page](https://careers.fylehq.com) that will give you a glimpse of what it is like to work at Fyle. Also, check out our Glassdoor reviews [here](https://www.glassdoor.co.in/Reviews/Fyle-Reviews-E1723235.htm). You can read stories from our teammates [here](https://stories.fylehq.com).


## Challenge outline

This challenge involves writing a backend service for a classroom. The challenge is described in detail [here](./Application.md)


## What happens next?

You will hear back within 48 hours from us via email. 


## Installation

1. Fork this repository to your github account
2. Clone the forked repository and proceed with steps mentioned below

### Installation Guide Video
[![](http://img.youtube.com/vi/m48VjM2EriY/0.jpg)](https://youtu.be/m48VjM2EriY)

### Install requirements

```
virtualenv env --python=python3.8
source env/bin/activate
pip install -r requirements.txt
```
### Reset DB

```
export FLASK_APP=core/server.py
rm core/store.sqlite3
flask db upgrade -d core/migrations/
```
### Start Server

```
bash run.sh
```
### Run Tests

```
pytest -vvv -s tests/

# for test coverage report
# pytest --cov
# open htmlcov/index.html
```
#### Test Video
[![](http://img.youtube.com/vi/dK_5G-FdluA/0.jpg)](https://youtu.be/dK_5G-FdluA)

#### Test Coverage Video
[![](http://img.youtube.com/vi/GdTFLauDztk/0.jpg)](https://youtu.be/GdTFLauDztk)

## Docker Setup

**If you don't have Docker installed, [see here](https://www.docker.com/products/docker-desktop/)**

### Installation
1. Fork this repository to your GitHub account.
2. Clone the forked repository and proceed with the steps mentioned below:

```bash
# Head over to the directory and type the following command
docker-compose run
# Now you can see your container is running
```
### Run Test
```
# Enter into the container shell
docker exec -it <container name> sh

# For container name, use
docker ps

# Run tests
pytest -vvv -s tests/

# For test coverage report
# pytest --cov
# Open htmlcov/index.html
```
### Stopping container
```
docker-compose down
```
### Docker Deployment link
[Click here](https://fyle-interview-intern-backend-latest.onrender.com/)
