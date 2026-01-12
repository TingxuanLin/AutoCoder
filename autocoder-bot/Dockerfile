# Stage 1: Build the application
FROM python:3.9-slim AS build-stage
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

# Stage 2: Create the final lightweight image
FROM python:3.9-slim
WORKDIR /app
COPY --from=build-stage /app/ .
CMD ["python", "app.py"]
