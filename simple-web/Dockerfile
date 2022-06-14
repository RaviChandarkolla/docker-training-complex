# Specify a base imahe
FROM node:alpine

WORKDIR /usr/app/

# Install some dependencies
# This step is for using of cache to reduce the rebuilding and preventing execution of npm install multiple times unnecessarily
COPY ./package.json ./
RUN npm install
COPY ./ /usr/app

# Default command
CMD ["npm", "start"]