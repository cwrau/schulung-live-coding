FROM python:3.10-alpine
WORKDIR /code
ENV FLASK_APP=backend.py
ENV FLASK_RUN_HOST=0.0.0.0
COPY ./requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
EXPOSE 5000
COPY . .
CMD ["flask", "run", "--debug"]
