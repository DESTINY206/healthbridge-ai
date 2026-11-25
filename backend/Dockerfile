FROM node:20-alpine

ENV NODE_ENV=production
WORKDIR /app

COPY backend/package.json backend/package-lock.json ./
RUN npm ci --omit=dev

COPY backend/src ./src

EXPOSE 4000
CMD ["npm", "start"]
