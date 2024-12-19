# Use an existing image as a base
FROM docker.io/node:18-alpine

# Create a Work Directory
WORKDIR /usr/app

#copy the package.json first
COPY ./package.json ./

# Run the command to install application dependencies
RUN npm install

#Copy the rest of the files to container
#Copy src(host/path) destination(container/path)
COPY ./ ./
 
# The command to run on container startup
# This will start the NodeJS app
CMD ["npm", "start"]
