FROM python:3.7-slim-stretch

# Mount volume
ADD ./src/ /app

# Set working directory
WORKDIR /app

# Install python dependencies
RUN python3 -m pip install -r requirements.txt
ENV FLASK_APP=server.py

# Hot reload flag
ENV FLASK_ENV=development

# Run flask app on port 8000
ENV FLASK_RUN_PORT=8000
CMD ["flask", "run", "--host", "0.0.0.0"]
