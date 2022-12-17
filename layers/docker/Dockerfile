FROM ubuntu

RUN apt-get update
RUN echo hihi
RUN touch /hi
RUN rm /hi
RUN touch a_file
WORKDIR /a_folder
RUN touch a_file
RUN ls -l
RUN echo $PWD $HOME
RUN apt-get install curl nmap net-tools dnsutils -y
CMD ["echo", "hello"]