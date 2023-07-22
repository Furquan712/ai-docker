# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (if applicable)
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Expose the port that the frontend application will run on
EXPOSE 3000

# Start the frontend application
CMD ["npm", "run dev"]
