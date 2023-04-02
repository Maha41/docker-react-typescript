# pull the base image
FROM node:12.18.3-alpine3.9

# set working directory
WORKDIR /react-typescript-starter

# add `/react-typescript-starter/node_modules/.bin` to $PATH
ENV PATH /react-typescript-starter/node_modules/.bin:$PATH

# install app dependencies
COPY package.json ./

COPY yarn.lock ./

RUN npm install --silent

# add app
COPY . ./

# start app
CMD ["npm", "start"]
