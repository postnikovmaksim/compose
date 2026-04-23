FROM python:3.11-slim

WORKDIR /app

# клонируем оригинал
RUN apt-get update && apt-get install -y git \
    && git clone https://github.com/berrykuipers/mcp_services_radarr_sonarr.git .

# установка
RUN pip install --no-cache-dir .

EXPOSE 3000

CMD ["python", "run.py"]