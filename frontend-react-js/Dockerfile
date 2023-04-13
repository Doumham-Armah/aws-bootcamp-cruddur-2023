FROM node:16.20

WORKDIR /frontend-react-js
COPY package*.json ./

RUN npm install
COPY . .

ENV PORT=3000
EXPOSE ${PORT}

CMD ["npm", "start"]