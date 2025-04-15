### Prerequisites
Git
Python
Docker
Visual Studio

### Create a folder 
for example
mkdir simple_time_service
cd simple_time_service

### Clone the Repository

git clone https://github.com/Praveen-devu/particle41.git
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
  
