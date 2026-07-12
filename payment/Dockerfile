FROM python:3.9
WORKDIR /app
COPY requirements.txt .
COPY payment.ini .
COPY *.py .
RUN pip install -r requirements.txt
COPY *.py .
EXPOSE 8080
CMD ["uwsgi", "--ini", "payment.ini"]