# LLM-based Automation Agent

## Overview
This project implements an automation agent powered by Large Language Models (LLM) to assist with various automation tasks. The agent is containerized using Docker for easy deployment and scalability.

## Prerequisites
- Docker installed on your system
- Valid AIPROXY_TOKEN (required for API authentication)
- Internet connection for pulling the Docker image

## Quick Start

### Environment Setup
1. Make sure you have your AIPROXY_TOKEN ready. 
2. Set your AIPROXY_TOKEN as an environment variable:
```bash
export AIPROXY_TOKEN=your_token_here
```

### Running the Agent
Execute the following Docker command to start the automation agent:
```bash
docker run -e AIPROXY_TOKEN=$AIPROXY_TOKEN -p 8000:8000 garriimaa/llm_automation
```

This command will:
- Pull the image if not already present locally
- Map port 8000 from the container to your host machine
- Pass your AIPROXY_TOKEN to the container
- Start the automation agent service

### Accessing the Service
Once the container is running, you can access the service at:
```
http://localhost:8000
```

## Configuration
The service uses the following default configurations:
- Port: 8000
- Container Image: garriimaa/llm_automation


## License
MIT License
