FROM node:20-alpine

WORKDIR /app

# Copy package files first (better caching)
COPY package*.json ./

# Install all dependencies (dev deps needed for dev server)
RUN npm install

# Copy rest of the application
COPY . .

# Expose dev server port (change if needed)
EXPOSE 5173

# Start dev server
CMD ["npm", "run", "dev", "--", "--host"]