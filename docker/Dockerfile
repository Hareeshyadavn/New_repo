FROM python:3.8-slim-buster
RUN apt update && apt install -y iputils-ping telnet dnsutils
WORKDIR /app
COPY dependency.txt ./
RUN pip install -r dependency.txt
COPY . .
CMD ["python", "demo.py"]
