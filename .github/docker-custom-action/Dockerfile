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

# Install shell (Alpine only has /bin/sh by default; if you need bash, install it)
RUN apk add --no-cache bash

# Copy the entrypoint script into the container
COPY entrypoint.sh /entrypoint.sh

# Make sure it’s executable
RUN chmod +x /entrypoint.sh

# Set entrypoint
ENTRYPOINT ["/entrypoint.sh"]


