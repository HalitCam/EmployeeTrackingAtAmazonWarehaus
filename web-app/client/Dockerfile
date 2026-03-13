FROM node:22-slim
WORKDIR /opt/amazon-lager/client
COPY . /opt/amazon-lager/client
ARG REACT_APP_BASE_ENDPOINT
ENV REACT_APP_BASE_ENDPOINT=$REACT_APP_BASE_ENDPOINT
ENV NODE_OPTIONS=--max-old-space-size=4096
RUN npm install
RUN npm run build
RUN npm install -g serve
EXPOSE 3000
CMD ["serve", "-s", "build", "-l", "3000"]