# Mailhog Docker Container for AARCH64, ARMv7l, X86 and X64

For using Mailhog with Docker.  
Mailhog is a handy SMTP mail server useful for local and team application development.  
You can use this image to send mail to a SMTP host
and Mailhog provides the SMTP server and web frontend.  
For more information on Mailhog please see Mailhog [Github Repository](https://github.com/mailhog/MailHog).

## Docker Container usage
- copy `docker-compose-<ARCH>-SAMPLE.yaml` to `docker-compose.yaml`
- edit the file if needed
- run `$ ./dc-m-mh.sh up`

To stop the container run `$ ./dc-m-mh.sh down`

## Email Client configuration
- SMTP port: 1025 (by default)
- SMTP Authentification required?: no
- SMTP via SSL or TLS?: no

## Web Frontend usage
Navigate to `http://localhost:8025` in your webbrowser.  
Note: if you modified the port that is mapped to port 8025 inside the container
you'll need replace "8025" in above URL with that port number.

## Required Docker Image
The Docker Image **mail-mailhog-\<ARCH\>** will automaticly be downloaded from the Docker Hub.  
The source for the image can be found here [https://github.com/tsitle/dockerimage-mail-mailhog](https://github.com/tsitle/dockerimage-mail-mailhog).

## Configuration
[Configure MailHog](CONFIG.md)  
Source: [https://github.com/mailhog/MailHog/blob/master/docs/CONFIG.md](https://github.com/mailhog/MailHog/blob/master/docs/CONFIG.md)
