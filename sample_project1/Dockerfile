# Use the official lightweight Python image.
FROM python:3.10-slim

# Set the working directory.
WORKDIR /app

# Copy the requirements file into the container.
COPY requirements.txt requirements.txt

RUN pip3 install -r requirements.txt

EXPOSE 8501

COPY . .

ENTRYPOINT ["streamlit", "run"]

CMD ["app.py"]
