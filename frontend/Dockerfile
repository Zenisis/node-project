

# Use an official Node.js runtime as a parent image
FROM node:14 AS build 

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire application to the container
COPY . .

# Build the React app
RUN npm run build



# Expose port 80 to the outside world
EXPOSE 3000

# Start NGINX when the container starts
CMD ["npm", "start"]
