# Docker Registry Setup
## Introduction

Create a Docker registry with TLS and HTPASSWD auth. Docker and Docker compose need to be installed on the host machine.

[Install Docker][docker-install]

[Install Docker Compose][docker-compose-install]
## Usage
### Setup

Clone this repo on the target machine and setup the required .env file.

```bash
git clone https://github.com/boxpositron/docker-registry-setup
cd docker-registry-setup
cp .env.example .env
```

### Customise
Edit the values for HTAUSER and HTPASS in the .env file generated in the previous step with your preferred editor.

### Deployment 

Deploying the registry server with docker-compose. 

```
docker-compose up -d
```

This registry container will be bound to port 443 of the host machine. 

[docker-install]: https://docs.docker.com/engine/install/
[docker-compose-install]: https://docs.docker.com/compose/install/