FROM ubuntu

RUN apt-get update
RUN echo hihi
RUN touch /hi
RUN rm -f /hi    #This layer has been created/updated/removed

## The following images will be rebuild
RUN apt-get install curl nmap net-tools dnsutils -y
RUN echo NEWLINE!!!
CMD ["echo", "hello"]