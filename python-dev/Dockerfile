FROM ubuntu:precise                                                                                                                                                                                
MAINTAINER Mattias Appelgren, mattias@ppelgren.se                                                                                                                                                  
                                                                                                                                                                                                   
RUN apt-get install -y python                                                                                                                                                                      
                                                                                                                                                                                                   
ADD https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py /tmp/                                                                                                                          
RUN python /tmp/ez_setup.py                                                                                                                                                                        
                                                                                                                                                                                                   
ADD https://raw.github.com/pypa/pip/master/contrib/get-pip.py /tmp/                                                                                                                                
RUN python /tmp/get-pip.py                                                                                                                                                                         
                                                                                                                                                                                                   
RUN pip install virtualenv
