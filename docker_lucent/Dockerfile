FROM postgres:16

# Environment variables
ENV POSTGRES_DB=notion_cms
ENV POSTGRES_USER=postgress
ENV POSTGRES_PASSWORD=Pass@123

# Copy schema file to auto-init directory
COPY schema.sql /docker-entrypoint-initdb.d/schema.sql

# Expose PostgreSQL port
EXPOSE 5432