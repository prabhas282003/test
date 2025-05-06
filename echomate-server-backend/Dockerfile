# Base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Install app dependencies
COPY package*.json ./
RUN npm install --production

# Copy app source code
COPY . .

# Expose the backend port
EXPOSE 3000

# Start the server
CMD ["npm", "start"]
