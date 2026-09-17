# Mock-API:t – en fristående Express-server. Inte med i frontend-builden.
FROM node:22-alpine
WORKDIR /app
COPY mock-api/server.js .
RUN npm install express
# API_KEY sätts av compose/miljön vid start. Saknas den skriver server.js ut fel.
EXPOSE 4000
CMD ["node", "server.js"]
