FROM node:current-alpine
EXPOSE 4000
WORKDIR /usr/src/app
ENV PUPPETEER_SKIP_CHROMIUM_DOWNLOAD true
COPY package*.json ./
COPY resume.json ./
RUN npm install
RUN npm install resume-cli -g
COPY . .
CMD [ "resume" , "serve"]
