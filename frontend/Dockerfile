FROM node:18
RUN npm install @angular/cli
WORKDIR /app/
COPY package*.json .
RUN npm install 
COPY . .
CMD ["ng", "serve", "--host", "0.0.0.0"]
