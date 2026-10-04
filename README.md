# Báo Cáo Khởi Tạo Local Repository Và Cấu Hình Danh Tính

## 1. Các Lệnh Đã Thực Hiện

### Bước 1: Khởi tạo Git repository cục bộ
```bash
git init -b main
```

### Bước 2: Cấu hình danh tính ở cấp độ cục bộ (`--local`)
> **Ràng buộc:** Sử dụng cờ `--local` để chỉ áp dụng cho dự án này, không ảnh hưởng cấu hình toàn cục (`--global`).
```bash
git config --local user.name "ToAnhTuan1806"
git config --local user.email "toanhtuan.18dz@gmail.com"
```

### Bước 3: Thêm tệp tin vào Staging Area và thực hiện Commit đầu tiên
```bash
# Đưa các tệp vào vùng chuẩn bị
git add .

# Thực hiện commit đầu tiên
git commit -m "feat: initial commit for local repository"
```

---

## 2. Kết Quả Kiểm Tra Cấu Hình Cục Bộ (`--local`)

### Kiểm tra từng trường:
```bash
git config --local user.name
# Kết quả: ToAnhTuan1806

git config --local user.email
# Kết quả: toanhtuan.18dz@gmail.com
```

### Lệnh in toàn bộ cấu hình cục bộ (`git config --local --list`):
```text
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
user.name=ToAnhTuan1806
user.email=toanhtuan.18dz@gmail.com
```

---

## 3. Lịch Sử Commit (`git log --oneline`)

Lệnh kiểm tra:
```bash
git log --oneline
```

Kết quả hiển thị:
```text
40829ad feat: initial commit for local repository
```
Commit đầu tiên đã được ghi nhận với đúng thông tin tác giả và thông điệp rõ nghĩa.
