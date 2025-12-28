# Use the official Node.js image as a base image
FROM node:14

# Set  working directory inside  container
WORKDIR /app

# Copy package.json and package-lock.json to  working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to  working directory
COPY . .

# Expose the port that your app is running on
EXPOSE 3500

# Command to run your application
CMD ["node", "server.js"]