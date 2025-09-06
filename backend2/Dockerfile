FROM node:18

WORKDIR /app

# Copy package.json and package-lock.json from current context (./backend2/src)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all source code
COPY . .

# Expose backend port
EXPOSE 5000

# Start the server
CMD ["node", "server.js"]
