FROM node:20-bullseye-slim

# Install system dependencies required to build native modules (better-sqlite3)
RUN apt-get update \
  && apt-get install -y --no-install-recommends \
    python3 \
    make \
    g++ \
    sqlite3 \
    libsqlite3-dev \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /usr/src/app

# Copy package files and install production dependencies
COPY package*.json ./
# Use npm install and omit dev deps to avoid strict lockfile requirements during container builds
RUN npm install --omit=dev --no-audit --no-fund

# Copy source
COPY . .

ENV NODE_ENV=production
ENV PORT=5000

EXPOSE 5000

CMD ["node", "server.js"]
