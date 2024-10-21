# Sử dụng Python làm base image
FROM python:3.9-slim

# Thiết lập thư mục làm việc
WORKDIR /app

# Copy file requirements.txt vào container
COPY requirements.txt .

# Cài đặt các thư viện
RUN pip install -r requirements.txt

# Copy mã nguồn
COPY . .

# Expose port 5000
EXPOSE 5000

# Chạy ứng dụng
CMD ["python", "app.py"]
