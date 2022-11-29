#Front
FROM node:16.18-bullseye
RUN apt -y update
RUN apt -y upgrade
RUN apt-get -y install  curl vim


# Montage des documents partagés
COPY ./my-vue-app/ /root/front/
WORKDIR /root/front
RUN npm install
EXPOSE 3000
ENV NUXT_HOST=0.0.0.0
ENV NUXT_PORT=3000
CMD ["npm", "run", "dev"]

