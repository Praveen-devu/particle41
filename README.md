# Task 1 - Minimalist Application Development / Docker / Kubernetes

### Prerequisites
Git

Python

Docker

Visual Studio

Make sure your docker is running while doing this entire process

### Create a folder 
example: 
mkdir simple_time_service

cd simple_time_service

### Clone the Repository

git clone https://github.com/Praveen-devu/particle41.git

cd particle41

git checkout simpletimeservice


### Build the Docker Image

docker build -t simple_time_service .

### Run the Container

docker run -p 5000:5000 simple_time_service

The app will now be accessible at http://localhost:5000

### Test the Service
Open your browser and hit http://localhost:5000/

### Expected response:
{
  "timestamp": "2025-04-15T12:34:56",
  "ip": "127.0.0.1"
}
  
