FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install --production

# Copy application source
COPY . .

# Explicitly copy .env to /app
COPY edit_env /app/.env

EXPOSE 5000

CMD ["node", "index.js"]