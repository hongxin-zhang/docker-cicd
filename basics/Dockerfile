FROM node:4.6 as unittest
RUN sleep 10
RUN echo "unit test"

FROM node:4.6 as codeanalysis
RUN sleep 10
RUN echo "coverage and static analysis"

FROM node:4.6 as uitest
RUN sleep 10
RUN echo "UI tests"

FROM node:4.6 as buildartifact
RUN sleep 10
RUN echo "final artifact"

WORKDIR /app
ADD . /app
RUN npm install
EXPOSE 3000
CMD npm start