#Front
FROM node:16.18-bullseye
RUN apt -y update
RUN apt -y upgrade
RUN apt-get -y install  curl vim


# Montage des documents partagés
COPY ./my-vue-app/ /root/front/
WORKDIR /root/front
RUN npm install
EXPOSE 5173
CMD ["npm", "run", "dev"]

