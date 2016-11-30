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

* Run the script:
  `./project start`

* Run tests:

 - You need to install moreutils package using the command:

    `$ apt-get install moreutils`

 - To run all tests execute the command:

    `./tests/run_all`
