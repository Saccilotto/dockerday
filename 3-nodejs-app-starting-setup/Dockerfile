FROM node

WORKDIR /app
# WORKDIR sets the directory context inside the image for the next instructions that follow in the Dockerfile.
COPY . /app
#COPY . /app(already set bt WORKDIR)
#COPY .(The place where the files should be copied in the external env of the container) .(the place inside the image/container it should be copied to). 
#In this case, we are copying the files from the external env to the /app directory inside the container.

RUN npm install
# RUN command defines a command to be run while the IMAGE is being BUILT.
 
EXPOSE 80

CMD ["node" , "node server.js"]
# CMD command defines a command to be run when the IMAGE will be actually executed as container after it starts.
# Should be the last command in the Dockerfile.