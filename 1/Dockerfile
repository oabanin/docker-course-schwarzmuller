FROM node

WORKDIR /app

#Better to copy package.json separately for caching steps
COPY package.json /app

RUN npm install

COPY .. /app
#SAME as . . if WORKDIR changed
#SAME as . ./ if WORKDIR changed



#Does not really do anything
#More like documentation
EXPOSE 80

#Dockerfile is the instruction for image
#RUN node server.js is wrong because it means that we want start server in template
#we only want to start the server only after container starts

#WHEN CONtAINER StARTED
#Always should be the last
CMD ["node", "server.js"]

#RUN for image
#CMD for contaoner