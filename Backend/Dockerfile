FROM node:20-alpine
WORKDIR /app

# Install production deps
COPY package*.json ./
RUN npm ci --only=production

# Copy source
COPY . .

EXPOSE 3102
CMD ["node", "server.js"]

