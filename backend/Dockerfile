# Use Node.js base image
FROM node:18-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application code
COPY . .

# Create directory for data files
RUN mkdir -p /app/data

# Expose backend port
EXPOSE 5000

# Start the backend app
CMD ["npm", "start"]