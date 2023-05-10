# <img height="25" src="./images/AILLogoSmall.png" width="40"/> Config-repo

<a href="https://www.legosoft.com.mx"><img height="150px" src="./images/ConfigRepoLogo.png" alt="AI Legorreta" align="left"/></a>
This repository contains all the configuration files (*.yml files) for all micro.services in the marketplace  "AI markeplace" 
for two platforms:
* Local no docker: `localNoDocker` platform tu run the microservice inside the IDE. 
* Local docker: `local` on-premise (docker desktop).

Other platforms does not use Spring Config Server but Kubernetes ConfigMAp & Secret.
## File structure

All config files follow the `Spring Config Server` where ii is as follows:

* <micro-service-name>.yml for `default` configuration different from application.yml, inside the proyect.
* <micro-service-name>-localNoDocker for configuration to run inside the IDE. All URLs are `localHost`.
* <micro-service-name>-local for configurations inside the `Docker desktop`, i.e., the container name.

This repository is utilized by the `config-service` microservice and are just for `Docker desktop` platform.

All the files are read using `gitHub` repository.

### Contact AI Legorreta

Feel free to reach out to AI Legorreta on [web page](https://legosoft.com.mx).

Version: 2.0
©LegoSoft Soluciones, S.C., 2023