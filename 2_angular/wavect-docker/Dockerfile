# Stage 1
FROM node:15.9.0 as builder

RUN mkdir -p /app
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . ./

RUN npm run build --prod


# Stage 2
FROM nginx

COPY --from=builder /app/dist/wavect-docker /usr/share/nginx/html