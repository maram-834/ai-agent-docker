# AI Agent

A Django chat application with an AI agent, packaged with Docker.

## Run it from this repository

1. Clone the repo:
   git clone https://github.com/maram-834/ai-agent-docker.git
   cd ai-agent-docker

2. Build the Docker image:
   docker build -t ai-agent .

3. Run the container (replace your_key with a valid API key):
   docker run -p 8000:8000 -e GEMINI_API_KEY=your_key ai-agent

4. Open http://localhost:8000

## Create an admin user

In a second terminal:
   docker ps
   docker exec -it CONTAINER_NAME python manage.py createsuperuser

Then log in at http://localhost:8000/admin