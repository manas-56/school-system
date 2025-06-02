# Stage 1: Build dependencies
FROM node:16-alpine

# Set working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm ci

# Copy app source
COPY . .

# Expose the port the app runs on
EXPOSE 3001

# Start the app
CMD ["npm", "start"]
