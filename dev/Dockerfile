# Use UBI 9 minimal as base
FROM registry.access.redhat.com/ubi9/ubi-minimal

# Install Python for a simple app example
RUN microdnf install -y python3 && microdnf clean all

# Create app directory
WORKDIR /app

# Create a simple Hello World app
RUN echo 'print("Hello from Tekton CI pipeline!")' > app.py

# Run the app
CMD ["python3", "app.py"]
