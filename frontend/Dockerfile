# latest node image
FROM node:latest

# set working directory
WORKDIR /app

# install dependencies and start dev server
COPY package.json package-lock.json ./
RUN npm install

COPY . .

EXPOSE 3000 

CMD ["npm", "run", "dev"]

