
# How to get your domain's certificate?

## step1: config your domain resolve to your server

Please refer the documentation of your domain name provider, add "A" record to resolve to your server's
ip address.

## step2: run certbot tool,get your certificate

1 Modify docker-compose.yml file 

In the line contains "command", you need to replace the -d parameter value with your domain name. oc, you can
have multiple -d parameters.

2 In ./certbot directory, run 

$ docker-compose up

You will see some output, If you notice some "Successfully received certificate." message, it means 
you have the certificate files. You are ready to the next step!
