<<<<<<< HEAD
FROM node:18-alpine
=======
# Stage 1: Build
FROM node:18 AS builder
>>>>>>> d7ca8bf60778961cffa6843a0007cfabf10aef4b
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build
<<<<<<< HEAD
EXPOSE 3000
CMD ["npm", "start"]
=======

# Stage 2: Serve
FROM nginx:alpine
COPY --from=builder /app/dist /usr/share/nginx/html
COPY nginx.conf /etc/nginx/nginx.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
>>>>>>> d7ca8bf60778961cffa6843a0007cfabf10aef4b
