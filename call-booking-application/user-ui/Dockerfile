FROM node:17.9.0-slim
LABEL maintainer = "Rishabh Alchetti"
RUN  useradd -m userui
WORKDIR /app
COPY . .
RUN chown -R userui:userui /app
USER userui
RUN npm install 
EXPOSE 3000
CMD ["npm","start"]