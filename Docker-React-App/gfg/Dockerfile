FROM node:20-alpine

WORKDIR  /app

COPY package*.json ./

#used for installing dependencies and reack packages  e.g React, React-DOM, Vite/React Scripts, etc
RUN npm install  

#copy your REACT application 
COPY . .
#the first dot '.' means take everything from the current folder and the second dot '.' means  add the to the cpntainer current working folder '/app'

EXPOSE 3000 
#tells docker to listen to port 3000

CMD ["npm", "start"]