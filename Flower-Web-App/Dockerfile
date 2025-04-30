# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json (if exists)
COPY Flower-Web-App/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY Flower-Web-App/ ./

# Expose the port the app will run on
EXPOSE 8000

# Define the command to run the app
CMD ["npm", "start"]
