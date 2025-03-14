# Task Management Application (ptud-gk-de-2)

## Thông tin cá nhân
- **Họ và tên**: Nguyễn Đăng Tuấn Huy
- **Mã số sinh viên**: 22658341
- **Lớp**: DHKHDL18A
- **Email**: huy298445@gmail.com

## Mô tả dự án
Đây là ứng dụng quản lý công việc (task) được xây dựng bằng Django, cho phép người dùng theo dõi và quản lý các công việc của họ. Ứng dụng có các chức năng chính như:

- Đăng ký, đăng nhập và quản lý tài khoản người dùng
- Tải lên và quản lý avatar (hình đại diện) cá nhân
- Thêm, sửa, xóa, và theo dõi các công việc (tasks)
- Hiển thị cảnh báo về các công việc trễ hạn
- Phân loại công việc theo danh mục (categories)
- Theo dõi trạng thái công việc (pending, in_progress, completed, cancelled)
- Ghi lại thời gian tạo và thời gian hoàn thành công việc

## Yêu cầu hệ thống
- Python 3.8 trở lên
- Django 4.0 trở lên
- Pillow (cho xử lý hình ảnh)
- Các thư viện khác được liệt kê trong file requirements.txt

## Hướng dẫn cài đặt

### 1. Clone repository
```bash
git clone https://github.com/your-username/ptud-gk-de-2.git
cd ptud-gk-de-2
```

### 2. Tạo và kích hoạt môi trường ảo
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python3 -m venv venv
source venv/bin/activate
```

### 3. Cài đặt các thư viện cần thiết
```bash
pip install -r requirements.txt
```

### 4. Thực hiện migrate để tạo cơ sở dữ liệu
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Tạo tài khoản admin
```bash
python manage.py createsuperuser
```

### 6. Chạy server
```bash
python manage.py runserver
```

Sau khi thực hiện các bước trên, bạn có thể truy cập ứng dụng tại `http://127.0.0.1:8000/`

## Cấu trúc dự án
- `taskmanager/`: Thư mục chính của dự án Django
- `tasks/`: Ứng dụng quản lý công việc
- `static/`: Chứa các file tĩnh (CSS, JavaScript, images)
- `media/`: Lưu trữ các file được người dùng tải lên (như avatar)

## Tính năng chính
1. **Quản lý người dùng**:
   - Đăng ký tài khoản mới
   - Đăng nhập/Đăng xuất
   - Cập nhật thông tin cá nhân và avatar
   
2. **Quản lý công việc**:
   - Thêm công việc mới
   - Chỉnh sửa công việc đã tạo
   - Xóa công việc
   - Xem chi tiết công việc
   
3. **Hiển thị công việc trễ hạn**:
   - Thông báo số lượng công việc trễ hạn gần avatar người dùng
   - Hiển thị danh sách công việc trễ hạn

4. **Dashboard**:
   - Tổng quan về các công việc
   - Thống kê theo trạng thái
   - Danh sách công việc gần đây
   
5. **Phân loại công việc**:
   - Tạo và quản lý các danh mục công việc
   - Gán công việc vào danh mục

## Giao diện
Ứng dụng sử dụng giao diện Single Column (Một Cột) để hiển thị dữ liệu một cách rõ ràng và dễ sử dụng.