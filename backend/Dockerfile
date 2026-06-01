FROM node:18-alpine

WORKDIR /usr/src/app

# Install dependencies from root package.json
COPY package.json ./
RUN npm install --production

# Copy backend source only
COPY backend ./backend
COPY uploads ./uploads

EXPOSE 5000

CMD ["npm", "run", "start"]
