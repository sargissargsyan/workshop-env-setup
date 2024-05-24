# Testing Environment Setup for Workshop

## Description
This project sets up a consistent testing environment for our coding workshop. It ensures every participant has the same testing tools and versions, reducing setup time and potential discrepancies in test results.

## Getting Started

### Prerequisites
Before the setup, ensure you have the following software installed on your machine:

- Java
- IntelliJ IDEA

### Setting up AWS instance for the project

1. Create an Ubuntu instance with 8GB and 32GB storage.
2. Make sure that the security group is configured to be accessible from the outside.
3. ssh to a created instance
4. Install docker and docker-compose running this command 
`sudo apt-get update && echo "Y" | sudo apt-get install docker.io && sudo curl -L "https://github.com/docker/compose/releases/download/1.28.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose && sudo chmod +x /usr/local/bin/docker-compose`

### Installation

1. Clone the project to your local machine using `git clone https://github.com/sargissargsyan/workshop-env-setup.git`.
2. Edit .env file and set the running machine IP for `TAIGA_DOMAIN`
3. Run `docker-compose -f docker-compose-taiga.yml up -d` to start the Taiga app
4. run `docker-compose -f docker-compose-v3-dynamic-grid.yml up -d` to start Selenium Grid



#### Links
| docker-taiga | [link](https://github.com/taigaio/taiga-docker) |
| docker-selenium | [link](https://github.com/SeleniumHQ/docker-selenium) |