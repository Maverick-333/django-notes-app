FROM node:16

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

