# This will install nodejs into alpine. So it will not only contain base alpine
FROM node:16-alpine

# Working directory of the linux
WORKDIR /usr/src/app

# Copy all package.json into the working dir
COPY package*.json ./

# Run the npm install command.
RUN npm install

# Copy entire folder from current directory to the Workdir.
# So basically copy all the file inside docker-playground into /usr/src/app
COPY . .

RUN npm run build

# Expose the docker port 3000
EXPOSE 3000

# Run the node server
CMD ["npx", "serve", "build"]