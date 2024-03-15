FROM nginx:alpine

WORKDIR /usr/share/nginx/html

COPY . /usr/share/nginx/html

# Set the environment variable to point to the backend service
ENV WS_BACK_URL=http://actual_backend_service_url:5000

# Entrypoint to start nginx in the foreground
ENTRYPOINT ["nginx", "-g", "daemon off;"]
