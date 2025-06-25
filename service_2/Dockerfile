FROM python:3.13-slim

WORKDIR /app

COPY . .

# Install required build tools
RUN pip install --upgrade pip setuptools

# Install Python dependencies from pyproject.toml
RUN pip install --no-cache-dir .

# Expose port
EXPOSE 8002

# Run the Flask app
CMD ["python", "app.py"]

