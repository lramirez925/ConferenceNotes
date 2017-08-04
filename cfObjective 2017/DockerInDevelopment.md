# Docker in Development
## By Geoff Bowers -- twitter @modius --company: Daemon

1.  Looking at the tool chain. 
1. Why Docker. 
    1. Continous delivery is desirable
    1. devops pipline
    1. docker helos buidlin standarised pipelinses
    1. Helos on borading due to easy local deployment. 
    1. Able to deploy customized environments 

1. Utilized tool chain. 
    1. Docker-Machine for local docker engines in virtualBox. 
        - Allows more control over docker for windows. 
    1. docker-compose
    1. docker-workbench
    1. Drives everything from version control (Everything in version control.)
1. First step is make a standard project structure. 
    1. Always git ready. (Everything in the git....)
    1. Near production ready. 
    1. Single app per container. (Modules. 1 web context.)
1. lucee docker file is always neds to be inherited. 
    1. References a lucee bnase image. 
    1. Copy project into var/www
1. Everything is vulnerable to be lost. Save configs to github and copy into the docker. 
    1. Alternative 

1. docker-compose.yml
    1. Volume is very important workbench allows you to 

1. Commmands run. 
    1. docker-compose build -- forces new build of app. 
    1. docker-compose 

1. Lucess with nginx
    1. industry standard nginx
    1. supervised within Docker image. 
    1. Proxy to ports 80/443
    1. Lucee admin blocked by default. 
    1. Controversial use of nginx in same image as lucee. 
    1. Alloys you to get rid of ports. 
    1. Docker WorkBench has a reverse proxy. 
 
1. In dockerfile 
    1. Can add env variables. 
        1. Like Java opts. 
        1. other env variables. 
    1. Alternatively you can do it in compose files. (Can be shared by related images. )
    





Project Structure. 
    1. Dockerfile
    Readme.
    config
        - lucee
    src/ 
        -files
    docker-compose.yml