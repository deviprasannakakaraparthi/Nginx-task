FROM python:3.10-slim

WORKDIR /app
COPY . .
RUN apt-get update && apt-get install -y curl
RUN pip install flask

EXPOSE 8002
CMD ["python", "app.py"]

