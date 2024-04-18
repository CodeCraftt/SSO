# Use official Node.js image as base
FROM node:14 as build

# Set working directory inside the container
WORKDIR /src

# Copy package.json and package-lock.json (if exists)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the React app
RUN npm run build


