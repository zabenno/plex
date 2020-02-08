FROM ubuntu:18.04
MAINTAINER zabenno

#Install add-apt-repository and add Handbrake repo.
RUN apt update 
RUN apt install software-properties-common -y
RUN add-apt-repository ppa:stebbins/handbrake-releases -y -u

#Install Handbrake.
RUN apt install handbrake-cli -y

#Remove changes that are no longer needed.
RUN apt remove software-properties-common -y
RUN rm -rf /etc/apt/source*

#Enter on commandline, this will be change when I know requirements.
ENTRYPOINT /bin/bash
