# Use the .NET runtime image with Linux
FROM mcr.microsoft.com/dotnet/runtime:7.0 AS base

COPY ./app /app/
COPY ./plang /plang/

WORKDIR /app

# Expose port 10000 for the webserver
EXPOSE %port%

# Command to run when the container starts
ENTRYPOINT ["/plang/plang", "run"]