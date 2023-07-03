FROM node:14-alpine3.10

LABEL version="1.0"
LABEL description="React Frontend for the Library API"

WORKDIR /app

COPY package.json .
COPY package-lock.json .

RUN npm ci --only=production

COPY . .

CMD ["npm", "start"]
