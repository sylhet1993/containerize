FROM docker.io/python:3.7
WORKDIR /app
COPY src/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
ENV GUNICORN_CMD_ARGS="--bind=0.0.0.0 --reload"
EXPOSE 8000
CMD [ "gunicorn", "server:app" ]# your code goes here ...
