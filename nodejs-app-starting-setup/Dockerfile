#  tell docker which base image is required to build this image
FROM node

# following command mentions where all the subsequent command should execute
WORKDIR /app

COPY package.json /app/

RUN npm install

# which files of local images should go into the image
# following command basically teslls docker that take all files and folder which exist in sames folder as dockerfile,
# and then copy those inside app folder of docker file system
COPY . /app

# following command is optional. But while we are running th container, we weill have to mention the port number.
EXPOSE 80

# diff between RUN and CMD is that CMD commands dont execute while image is being built. CMD commands are only 
# used when we need to start the container based of the image
CMD ["node","server.js"]




