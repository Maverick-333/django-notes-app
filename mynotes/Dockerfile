FROM node:16

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 8000

#CMD ["npm", "start"]
CMD ["gunicorn", "notesapp.wsgi", "--bind", "0.0.0.0:8000"]


