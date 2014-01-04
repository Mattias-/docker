FROM ubuntu:precise
MAINTAINER Mattias Appelgren, mattias@ppelgren.se

# Set locale to UTF-8
RUN locale-gen en_US.UTF-8
RUN update-locale LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
ENV LANG en_US.UTF-8
ENV LC_ALL en_US.UTF-8

# Update python
RUN apt-get install -y python

# Install ez setup
ADD https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py /tmp/
RUN python /tmp/ez_setup.py

# Install pip
ADD https://raw.github.com/pypa/pip/master/contrib/get-pip.py /tmp/
RUN python /tmp/get-pip.py

# Install virtualenv
RUN pip install virtualenv
