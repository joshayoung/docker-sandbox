# docker-sandbox

### Docker Container for Testing Ansible
* Build and run with docker:
  * `docker build -t docker-sandbox .`
  * `docker run --name docker-sandbox-container -it -v "$(pwd)":/app --rm docker-sandbox`
* Build and run with docker-compose
  * `docker-compose build`
  * `docker-compose run --rm sandbox`
