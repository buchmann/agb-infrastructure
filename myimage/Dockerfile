############################################################
# Dockerfile to build Python WSGI Application Containers
# Based on Ubuntu
############################################################

# Set the base image to Ubuntu
FROM ubuntu:16.04

# File Author / Maintainer
MAINTAINER Maintaner Name

RUN apt-get update

RUN apt-get install -y tar git curl nano wget dialog net-tools build-essential

EXPOSE 5000

# Install Python and Basic Python Tools
RUN apt-get install -y python python-dev python-distribute python-pip

# Upgrade pip
RUN pip install --upgrade pip

# Install Flask
RUN pip install flask

# Run hello world app
RUN /usr/bin/python  
 
# Create App Dir
RUN cd /home

# Clone Python stuff 
RUN git clone https://github.com/buchmann/agb-infrastructure.git

# RUN Server 
RUN python /agb-infrastructure/myimage/myapp/hello.py



