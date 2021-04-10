## Build the image based npm:14 
FROM node:14

## Copy all the packages
COPY package*.json ./src/

## Change the default folder 
WORKDIR /usr/src/

## Install all packages
RUN npm install 

## Default port is 3000
EXPOSE 3000 

# Bundle app source
COPY . .

# Start all packages
RUN npm start

## When contianer is stared python app.py 
CMD ["node", "000.js"]
