FROM debian

MAINTAINER fepinson <fepinson@42.student.us.org>

ENV TS3SERVER_LICENCE=accept

WORKDIR /home/teamspeak

RUN apt-get update && apt-get upgrade &&\
	apt-get install -y wget bzip2 &&\
	wget http://dl.4players.de/ts/releases/3.0.13.4/teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2 && \
	    tar -xvf teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2

WORKDIR teamspeak3-server_linux_amd64

ENTRYPOINT sh ts3server_minimal_runscript.sh
