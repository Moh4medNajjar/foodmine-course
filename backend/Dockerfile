# Use the official Node.js 18 image as the base image
FROM node:18

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the TypeScript code
RUN npm run build  # This runs the build script defined in package.json

# Expose the port your app runs on
EXPOSE 5000

# Command to run the application
CMD ["node", "dist/src/server.js"]  # Adjust this if necessary
