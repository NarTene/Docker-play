# specify a base image
FROM ubuntu

#Then, install all the dependencies in the same file to be used by the image. 
RUN apt update
RUN apt install python3-pip -y
RUN pip3 install flask

# specify a directory and a name for the rest of its operations
WORKDIR /app


# copy the remainder of the files in our local working directory to the directory in the docker image.
COPY . .


# tell docker to run the flask app as module. Then, make the container available externally. 
CMD ["python3", "-m" , "flask", "run", "--host=0.0.0.0"]















