# Latest version of ubuntu as base image
FROM ubuntu:latest

# Get programs with Advanced Package Tool (APT)
RUN apt-get update
RUN apt-get upgrade -y

# Run commands
CMD ["echo", "Hello, World!"]

# Build me: docker build -f ./Dockerfile -t softy-pinko:task0 .
# Run me: docker run -it --rm --name softy-pinko-task0 softy-pinko:task0