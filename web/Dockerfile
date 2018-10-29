FROM debian:jessie-20181011

#
# Install node
#
RUN apt-get update
RUN apt-get -y install apt-transport-https curl
RUN curl -sL https://deb.nodesource.com/setup_8.x | bash -
RUN apt-get install -y nodejs

#
# Install useful terminal stuff
#

RUN apt-get install nano

#
# Create a project sharepoint and expose it 
#
RUN mkdir -p /var/www/project
VOLUME ["/var/www/project"]

#
# Expose ports
#
EXPOSE 80 8080
