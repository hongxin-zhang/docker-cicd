FROM node:4.6 as unittest
WORKDIR /app
ADD . /app
RUN echo "unit test"
FROM node:4.6 as codeanalysis
RUN echo "coverage and static analysis"
FROM node:4.6 as uitest
RUN echo "UI tests"
FROM node:4.6 as buildartifact
RUN echo "final artifact"
RUN npm install
EXPOSE 3000
CMD npm start