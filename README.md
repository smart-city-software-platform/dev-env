# Setup

* Clone the repository
* Init submodules:
  `git submodule init`
* Update submodules:
  `git submodule update`

TODO: we need to start services in a specific order
  - resource-adaptor
  - resource-cataloguer
  - data-collector
  - resource-viewer

Configure docker compose to run without root permission:

1- Add this line end of /etc/default/docker:
   `DOCKER_OPTS="-H tcp://127.0.0.1:4243 -H unix:///var/run/docker.sock"`
2- Add this line end of ~/.bashrc:
  `export DOCKER_HOST=tcp://localhost:4243`
3- Restart docker service:
  `sudo service docker restart`

* Run the script:
  `./project start`

* Run tests:

 - You need to install moreutils package using the command:

    `$ apt-get install moreutils`

 - To run all tests execute the command:

    `./tests/run_all`
