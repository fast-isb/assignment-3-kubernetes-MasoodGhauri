# Use an official Node.js runtime as the base image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /app/frontend

# Copy package.json and package-lock.json to the working directory
COPY frontend/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY frontend/ .

# Expose port to the outside world
EXPOSE 3002

# Define the command to run the application
CMD ["npm", "start"]
