FROM node:17.9.0-slim
LABEL maintainer="Rishabh"
RUN  useradd -m userapi
WORKDIR /app
COPY . .
RUN chown -R userapi:userapi /app
USER userapi
RUN npm install
EXPOSE 1004
ENV MONGO_URL = ""
ENV ADMIN_EMAIL = ""
CMD ["npm","start"]