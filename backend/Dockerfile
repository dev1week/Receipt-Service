# Base Image
FROM python:3

# Working Directory
WORKDIR /app

# Copy source code to working directory
COPY . .

# Install packages from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
VOLUME ./data
# Port
EXPOSE 8000


# Run Django server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000", "--noreload"]
#CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stock.wsgi:application"]