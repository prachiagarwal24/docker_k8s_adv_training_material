#silent installation, interactive mode is not possible in dockers but some servers use only interaction 
#eg. apache, weblogic want to pass variables at runtime
#if at all you want to pass variables u need to  do it using env variables

FROM ubuntu 

RUN apt-get update

RUN DEBIAN_FRONTEND=noninteractive apt-get install -y apache2

RUN DEBIAN_FRONTEND=noninteractive apt-get install -y apache2-utils

EXPOSE 80

CMD ["apachectl" , "-D" , "FOREGROUND"]

