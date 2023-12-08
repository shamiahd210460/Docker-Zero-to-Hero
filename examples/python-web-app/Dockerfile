FROM ubuntu:20.04

# Install Python and pip
RUN apt-get update && \
    apt-get install -y python3 python3-pip

# Show installed versions
RUN python3 --version
RUN pip3 --version

# Copy the application files
COPY . /app

# Set the working directory
WORKDIR /app

# Install dependencies
RUN pip3 install -r requirements.txt

# Verify the 'devops' directory exists
RUN ls -l devops

# Set the entry point
CMD ["python3", "app.py"]






