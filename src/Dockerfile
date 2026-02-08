FROM node:20-alpine

WORKDIR /app

# Copy dependency files first (better caching)
COPY package*.json ./

RUN npm install --production

# Copy rest of the source
COPY . .

EXPOSE 3000

CMD ["node", "server.mjs"]
