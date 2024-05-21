# Testing Environment Setup for Workshop

## Description
This project sets up a consistent testing environment for our coding workshop. It ensures every participant has the same testing tools and versions, reducing setup time and potential discrepancies in test results.

## Getting Started

### Prerequisites
Before the setup, ensure you have the following software installed on your machine:

- Java
- IntelliJ IDEA 

### Installation

1. Clone the project to your local machine using `git clone <Repo-URL>`.
2. Edit .env file and set the running machine IP for `TAIGA_DOMAIN`
3. Run `docker-compose -f docker-compose-taiga.yml up -d` to start the Taiga app
4. run `docker-compose -f docker-compose-v3-dynamic-grid.yml up -d` to start Selenium Grid



#### Links
| docker-taiga | [link](https://github.com/taigaio/taiga-docker) |
| docker-selenium | [link](https://github.com/SeleniumHQ/docker-selenium) |