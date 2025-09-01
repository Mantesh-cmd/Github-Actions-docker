# FROM node:16

# ENV MONGODB_CONNECTION_PROTOCOL mongodb+srv
# ENV MONGODB_DB_NAME gha-demo1
# ENV MONGODB_CLUSTER_ADDRESS  cluster0.lqqdtgh.mongodb.net
# ENV MONGODB_USERNAME maximilian
# ENV MONGODB_PASSWORD eI3R3UfNlJgWJe17

# WORKDIR /app

# COPY package*.json .

# RUN npm install

# COPY . .

# CMD ["npm", "start"]


# Container image that runs your code
FROM alpine:3.10

RUN chmod +x entrypoint.sh
# Copies your code file from your action repository to the filesystem path `/` of the container
COPY entrypoint.sh /entrypoint.sh

# Code file to execute when the docker container starts up (`entrypoint.sh`)
ENTRYPOINT ["/entrypoint.sh"]

