# Dockerfile for Vidora Angular Frontend
FROM node:20-alpine AS build
WORKDIR /app
COPY . .
RUN npm install && npm run build -- --output-path=dist

FROM nginx:alpine
COPY --from=build /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]