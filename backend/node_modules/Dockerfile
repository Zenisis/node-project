# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the application dependencies
RUN npm install

# Copy all local files to the container
COPY . .

# Expose the necessary ports
EXPOSE 3000 3001

# Define the command to run your applications
CMD ["npm", "start"]
