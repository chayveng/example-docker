# Use the official PostgreSQL image as the base
FROM postgres:latest

# Set environment variables for PostgreSQL
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=12345678
ENV POSTGRES_DB=example

# Expose the PostgreSQL port
EXPOSE 5432

# Copy custom initialization scripts to the container
COPY init.sql /docker-entrypoint-initdb.d/

# Start the PostgreSQL server when the container starts
CMD ["postgres"]

