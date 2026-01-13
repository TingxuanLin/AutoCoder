FROM python:3.9-slim as builder
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
RUN chmod +x entrypoint.sh
FROM python:3.9-slim
WORKDIR /app
COPY --from=builder /app/ .
CMD ["./entrypoint.sh"]
