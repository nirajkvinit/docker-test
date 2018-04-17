# Use an official python runtime as a parent image
FROM python:2.7-slim

#set the working directory to /app
WORKDIR /app

#Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

#make port 8080 available to the world outside this container
EXPOSE 8080

#define enviroment variable
ENV NAME World

#run app.py when the container launches
CMD ["python", "app.py"]
