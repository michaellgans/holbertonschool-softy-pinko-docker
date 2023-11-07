# Latest version of ubuntu as base image
FROM ubuntu:latest

# Get programs with Advanced Package Tool (APT)
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask flask-cors

# Where are we?
WORKDIR /app
COPY api.py /app/api.py

# Run commands
CMD ["python3", "/app/api.py"]

# Build me: docker build -f ./back-end/Dockerfile -t softy-pinko-back-end:task3 ./back-end
# Run me: docker run -p 5252:5252 -it --rm --name softy-pinko-back-end-task3 softy-pinko-back-end:task3