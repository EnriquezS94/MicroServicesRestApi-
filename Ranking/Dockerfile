FROM node:8

# Create app directory

WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./

RUN npm install
RUN npm install nodemon -g

#Bundle app source
COPY . .

# Expose port 3004
EXPOSE 3004
CMD [ "npm", "i" ]
CMD [ "npm", "install", "nodemon", "-g" ]
CMD [ "npm", "run", "dev" ]

