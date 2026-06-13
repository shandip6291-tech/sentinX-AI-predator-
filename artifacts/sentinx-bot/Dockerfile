FROM node:20-slim

WORKDIR /app

COPY package.json ./
RUN npm install -g pnpm && pnpm install

COPY . .

RUN pnpm run build

CMD ["pnpm", "run", "start"]
