# Setup

* Clone the repository
* Init submodules:
  `git submodule init`
* Update submodules:
  `git submodule -q foreach git pull -q origin master`

TODO: we need to start services in a specific order
  - resource-adaptor
  - resource-cataloguer
  - data-collector
  - resource-viewer

* Run the script:
  `./project start`
