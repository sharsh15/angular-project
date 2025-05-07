# Base image: Nginx
FROM nginx:alpine

# Remove default files
RUN rm -rf /usr/share/nginx/html/*

# Copy your pre-built Angular files into Nginx web directory
COPY dist/sample-angular-17-project /usr/share/nginx/html

# Expose port 80 for the web
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]