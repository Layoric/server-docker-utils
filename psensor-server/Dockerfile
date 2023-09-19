# Use a base Debian image
FROM ubuntu:22.04

# Update the package list and install psensor-server
RUN apt update && \
    apt install -y lm-sensors && \ 
    apt install -y psensor psensor-server

# Expose the default port for psensor-server
EXPOSE 7634

# Command to run psensor-server
CMD ["psensor-server","-p","7634","-d","3"]

