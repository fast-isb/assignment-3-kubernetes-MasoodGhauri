# Use the specific Node.js runtime version as the base image
FROM node:20.11.0-alpine

# Set the working directory in the container
WORKDIR /app/backend

# Copy package.json and package-lock.json to the working directory
COPY package.json package-lock.json ./

# Install dependencies with verbose logging for better error information
RUN npm install --verbose

# Copy the rest of the application code to the working directory
COPY . .

# Expose port to the outside world
EXPOSE 8003

# Define the command to run the application
CMD ["npm", "start"]
