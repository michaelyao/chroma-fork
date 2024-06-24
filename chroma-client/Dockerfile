FROM python:latest

RUN apt-get update && apt-get install -y \
                                        curl \
                                        iproute2
WORKDIR /app
COPY requirements.txt /app/
RUN pip install -r requirements.txt
COPY . /app/
CMD ["python"]