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
* For MacOS the `ansible_os_family` is equal to `Darwin`.

#### Resources:
* https://www.talkingquickly.co.uk/2021/01/macos-setup-with-ansible/
* https://www.handsonarchitect.com/2017/07/setup-macbook-almost-at-speed-of-light.html
* https://adamj.eu/tech/2019/03/20/how-i-provision-my-macbook-with-ansible/
  * https://github.com/adamchainz/mac-ansible
* https://towardsthecloud.com/automatically-setup-macbook-development 
  * https://github.com/geerlingguy/mac-dev-playbook
* https://gist.github.com/mrlesmithjr/f3c15fdd53020a71f55c2032b8be2eda
* https://austincloud.guru/2020/05/07/automating-macos-configuration/
* https://pythops.com/post/setup-your-linux-workstation-with-ansible.html
* https://www.talkingquickly.co.uk/2021/01/macos-setup-with-ansible/