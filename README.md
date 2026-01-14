# BÀI THỰC HÀNH TUẦN 1 – KIỂM THỬ PHẦN MỀM

Thông tin sinh viên

Họ và tên: Nguyễn Hồng Nhung

MSSV: BIT230308

Email: hiennguyen2270@gmail.com

Môn học: Kiểm thử phần mềm

Giảng viên: Trương Anh Hoàng

Mục tiêu bài thực hành
Làm quen với GitHub và cách quản lý bài thực hành bằng kho lưu trữ

Trải nghiệm và đánh giá chất lượng giao diện phần mềm

Nhận thức được vai trò của trải nghiệm người dùng (UX/UI) trong kiểm thử phần mềm

Nội dung thực hành
Trải nghiệm kiểm thử giao diện với CantUnsee
Truy cập website: https://cantunsee.space/

Thực hiện các bài kiểm tra phân biệt màu sắc và khả năng nhận diện giao diện

Minh chứng kết quả
Ảnh chụp màn hình kết quả làm bài trên Cantunsee

Ảnh có dấu hiệu cá nhân (ví dụ: đang đăng nhập Chrome)

Hình ảnh minh chứng:
![z7399927139999_37aa280ed691d6c1a0f452a90d62dcb0](https://github.com/user-attachments/assets/ae90a0b2-8b3b-430a-bcc3-a5499d4497a2)

# Bài tập thực hành tuần 2 kiểm thử với JUnit – Phân tích dữ liệu điểm số học sinh

## 1. Giới thiệu

Dự án này xây dựng một chương trình Java đơn giản để phân tích điểm số học sinh và viết kiểm thử đơn vị bằng **JUnit 5**.

### Mục tiêu học tập
- Biết cách viết Unit Test với JUnit.
- Áp dụng kiểm thử cho các trường hợp:
  - Bình thường
  - Biên
  - Dữ liệu không hợp lệ
- Biết cách tổ chức source code và test code trong repository.
- Thực hành quản lý công việc bằng GitHub Issues và Commit message.

---

## 2. Mô tả bài toán

Chương trình có lớp `StudentAnalyzer` với 2 phương thức:

### 2.1 countExcellentStudents(List<Double> scores)

- Đếm số học sinh có điểm **>= 8.0**
- Chỉ tính các điểm hợp lệ trong khoảng **0 – 10**
- Bỏ qua:
  - Điểm < 0
  - Điểm > 10
- Nếu danh sách rỗng → trả về `0`

### 2.2 calculateValidAverage(List<Double> scores)

- Tính điểm trung bình các điểm hợp lệ (0 – 10)
- Bỏ qua điểm không hợp lệ
- Nếu không có điểm hợp lệ → trả về `0`

---

## 3. Cấu trúc thư mục

unit-test/
│
├── src/
│ └── StudentAnalyzer.java
│
├── test/
│ └── StudentAnalyzerTest.java
│
└── README.md







