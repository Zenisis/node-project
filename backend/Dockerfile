# Use the official Node.js image as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package.json package-lock.json /app/

# Install dependencies
RUN npm install

# Copy all files from the current directory to the working directory
COPY . /app/

# Expose the port that the application will run on
EXPOSE 3001

# Define the command to run your application
CMD ["node", "server.js"]

