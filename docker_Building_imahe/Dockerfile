# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the current directory contents into the container at /usr/src/app
COPY . .

# Install any needed packages specified in package.json
RUN npm install

# Make your app available on the specified port
EXPOSE 8080

# Define environment variable
ENV NODE_ENV=production

# Run the app when the container launches
CMD ["node", "app.js"]
