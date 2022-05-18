FROM node:4.6 as unittest
WORKDIR /app
ADD . /app

FROM node:4.6 as coverage
EXEC sleep 10
RUN echo "Run coverage"

FROM node:4.6 as unitest
EXEC sleep 10
RUN echo "Run unit tests"

FROM node:4.6 as finalartifact
EXEC sleep 10
RUN echo "produce artifact"

RUN npm install
EXPOSE 3000
CMD npm start
