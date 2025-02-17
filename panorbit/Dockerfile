# Step 1: Use an official Python runtime as a parent image
FROM python:3.7.2-slim

# Step 2: Set the working directory in the container
WORKDIR /app

# Step 3: Copy the current directory contents into the container at /app
COPY . /app

# Step 4: Install the necessary dependencies
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Step 5: Expose the port the app will run on
EXPOSE 8001

# Step 6: Run the application
CMD ["python", "manage.py", "runserver", "0.0.0.0:8001"]
