<h1 align='center'>Microservice that calculates tax data in México</h1>

<div align='center'>
    <img src=https://github.com/thomgonzalez/taxdatamx/blob/develop/docs/images/API.png> 
</div>

What are tax data?
------------------
Tax data is the information that the Tax Administration Service has about you, such as identification data, tax address, branches and establishments of your business, your tax characteristics and information complementary to these.

## Technology Used
- [`Docker`](https://www.docker.com/) - Main tools to build this project
- [`FastAPI`](https://fastapi.tiangolo.com/) - Web framework for building APIs with Python
- [`Uvicorn`](https://www.uvicorn.org/)- Is an ASGI web server implementation for Python
- [`Python`](https://www.python.org/downloads/release/python-380/) - Programming language widely used in web applications, software development, data science and machine learning (ML)
- [`Pyfiscal`](https://github.com/sutsantiago/pyfiscal) - Library that calculates tax data

## Getting Started with Docker
If you want to install the dependencies and work using Docker, you can simply follow this steps. 

Clone the project repository

## Usage
There are several ways to use the project because there are those using `docker-compose.yml` and `Dockerfile`. Here's how to use it:

> This is for the install part with docker-compose
```compose
docker-compose up -d
````

> To stop service from docker-compose
```compose
docker-compose down
```

> Section to install with Dockerfile
```
$ docker build -t (name_image) .
```

## Run with Docker Hub

### Download precreated image 
You can also just download the existing image from [DockerHub](https://hub.docker.com/r/sutsantiago/taxdatamx).
```
docker pull sutsantiago/taxdatamx
```

### Run the container
Create a container from the image.
```
$ docker run --name my-container -d -p 8000:8000 sutsantiago/taxdatamx
```

Now visit http://localhost:8000

## LICENSE
Distributed under the MIT License. See [`LICENSE`](https://github.com/sutsantiago/taxdatamx/blob/main/LICENSE) for more information
