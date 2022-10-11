# Ansible-Nodejs-Deployer


<img src = "https://d7umqicpi7263.cloudfront.net/img/product/542db327-b437-4851-8f65-f15d5c80b4ef/e19a9f66-7cd7-4114-a2f1-6d43b77310e2.png" width ="250" /> <img src = "https://logos-download.com/wp-content/uploads/2016/09/Node_logo_NodeJS.png" width ="250" />

Ansible-Nodejs-Deployer is a sample project template which you can use to deploy your Node.js application on large number of linux machines.
This project is all written in yaml. I have used variables, conditions, loops and ansible built-in modules.

You should change variables and names to suit your needs.

The file structure is as follow:

- **certificates**: Contains TLS certificates.

- **docker-compose**: Contains docker compose files for services to deploy.

- **Dockerfile**: Contains Dockerfiles for micro-services we're going to deploy.

- **envs**:  Contains environment variables and secrets which is needed by micro-services.

- **nginx**: Contains nginx webserver config files.

- **main.yml**: This is the Ansible yaml file we use to deploy our code.

- **vars.yml**: Contains all environment variables used in main.yml.

## Requirements
You need to run this script on a system with Ansible, python, docker and git available available. Your Ansible version must be at least 2.9.

## Deployment
To run ansible just execute:
```bash
ansible-playbook main.yml
```
