# docker-sandbox

### Docker Container for Testing Ansible
* Build and run with docker:
  * `docker build -t docker-sandbox .`
  * `docker run --name docker-sandbox-container -it -v "$(pwd)":/app --rm docker-sandbox`
* Build and run with docker-compose
  * `docker-compose build`
  * `docker-compose run --rm sandbox`

#### Run Ansible Playbook
* `ansible-playbook setup.yml`

#### Notes:
* Run Mac in Docker: 
  * https://github.com/sickcodes/Docker-OSX#initial-setup
* universal-ctags:
  * Cannot be installed via snap in docker for testing, since snap does not seem work within docker.

#### Resources:
* https://www.talkingquickly.co.uk/2021/01/macos-setup-with-ansible/
