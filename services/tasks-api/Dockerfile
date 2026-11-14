from python:3.12-slim
workdir /app
copy requirements.txt .
run pip install --no-cache-dir -r requirements.txt
copy . .
expose 5000
cmd ["flask", "--app", "app:create_app", "run", "--host", "0.0.0.0", "--port", "5000"]