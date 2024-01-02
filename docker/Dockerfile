FROM honkit/honkit

WORKDIR /honkit-plugin

RUN apt-get -y update && apt-get -y upgrade
RUN apt-get -y install build-essential openjdk-17-jre graphviz

COPY ./package.json ./package.json
RUN yarn

ENV NODE_PATH=/honkit-plugin/node_modules:$NODE_PATH

CMD [ "npx honkit build" ]

