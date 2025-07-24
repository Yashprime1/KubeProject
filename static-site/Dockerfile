# Use the official Nginx image as base
FROM nginx:alpine

# Remove the default Nginx website
RUN rm -rf /usr/share/nginx/html/*

# Copy our static website files to the Nginx html directory
COPY index.html /usr/share/nginx/html/

# Copy custom Nginx configuration (optional)
# COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 80
EXPOSE 80

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]

# Optional: Add labels for better container management
LABEL maintainer="yashdeep@clevertap.com"
LABEL description="Static HTML website served with Nginx"
LABEL version="1.0"