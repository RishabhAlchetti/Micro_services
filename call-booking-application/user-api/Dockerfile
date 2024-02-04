FROM node:17.9.0-slim
LABEL maintainer="Rishabh"
RUN RUN useradd -m userapi
WORKDIR /app
COPY . .
RUN chown -R userapi:userapi /app
RUN npm install
EXPOSE 1004
USER userapi
ENV MONGO_URL = ""
ENV ADMIN_EMAIL = ""
CMD ["npm","start"]