FROM node:21

ENV NODE_OPTIONS=--max_old_space_size=2048

WORKDIR /app

RUN mkdir frontend
WORKDIR /app/frontend

COPY package-lock.json .
COPY package.json .
RUN npm i

COPY . .

EXPOSE 3000

CMD ["npm", "run", "dev"]