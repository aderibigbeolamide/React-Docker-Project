FROM node:18.12.0-alpine3.16

# RUN addgroup app && adduser -S -G app app
# RUN mkdir -p /home/app && chown -R app:app /home/app
# USER app

WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . . 

EXPOSE 3001 

CMD ["npm", "start"]