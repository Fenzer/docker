FROM debian
RUN apt-get update && apt-get install -y git ruby mysql-server
RUN git clone https://gitlab.com/gitlab-org/gitlab-foss.git
RUN sudo apt-get update
RUN sudo apt-get install -y curl openssh-server ca-certificates
RUN sudo apt-get install -y postfix
RUN sudo apt-get install -y curl
RUN curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash

