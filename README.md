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


<img width="1574" height="1045" alt="Screenshot 2026-01-14 140139" src="https://github.com/user-attachments/assets/edd17e4f-19a6-4967-bf00-264be5f0f461" />

# Bài tập thực hành 3 kiểm thử tự động End-to-End với Cypress – Website SauceDemo

## 1. Giới thiệu

Dự án này xây dựng các kịch bản kiểm thử tự động End-to-End cho website mẫu [https://www.saucedemo.com](https://www.saucedemo.com) bằng công cụ **Cypress**.

### Mục tiêu học tập

* Làm quen với kiểm thử tự động End-to-End.
* Biết cách cài đặt và sử dụng Cypress.
* Viết test case cho các chức năng phổ biến của website thương mại điện tử.
* Tổ chức mã nguồn và file kiểm thử trong repository.
* Thực hành quản lý source code bằng Git và GitHub.

---

## 2. Mô tả bài toán

Website SauceDemo mô phỏng một cửa hàng trực tuyến với các chức năng chính:

* Đăng nhập hệ thống
* Xem danh sách sản phẩm
* Thêm và xóa sản phẩm khỏi giỏ hàng
* Sắp xếp sản phẩm theo giá
* Thực hiện quy trình thanh toán

Sinh viên cần xây dựng các kịch bản kiểm thử tự động để kiểm tra các chức năng trên.

---

## 3. Các kịch bản kiểm thử

### 3.1 Kiểm thử đăng nhập thành công

* Truy cập trang web
* Nhập tài khoản hợp lệ: standard_user / secret_sauce
* Nhấn nút Login
* Kiểm tra chuyển hướng đến trang danh sách sản phẩm

### 3.2 Kiểm thử đăng nhập thất bại

* Nhập tài khoản không hợp lệ
* Nhấn nút Login
* Kiểm tra hiển thị thông báo lỗi

### 3.3 Kiểm thử thêm sản phẩm vào giỏ hàng

* Đăng nhập hệ thống
* Thêm một sản phẩm vào giỏ hàng
* Kiểm tra số lượng sản phẩm trong giỏ hàng

### 3.4 Kiểm thử sắp xếp sản phẩm theo giá

* Chọn bộ lọc Price (low to high)
* Kiểm tra sản phẩm có giá thấp nhất hiển thị đầu tiên

### 3.5 Kiểm thử xóa sản phẩm khỏi giỏ hàng

* Thêm sản phẩm vào giỏ hàng
* Nhấn Remove
* Kiểm tra giỏ hàng trống

### 3.6 Kiểm thử quy trình thanh toán

* Thêm sản phẩm vào giỏ hàng
* Đi tới trang giỏ hàng
* Thực hiện Checkout
* Nhập thông tin khách hàng
* Kiểm tra chuyển đến trang xác nhận thanh toán

---

## 4. Cấu trúc thư mục

```
cypress-exercise/
│
├── cypress/
│   └── e2e/
│       ├── login_spec.cy.js
│       └── cart_spec.cy.js
│
├── cypress.config.js
├── package.json
└── README.md
```

---

## 5. Cài đặt và chạy chương trình

### 5.1 Cài đặt môi trường

* Node.js phiên bản 14 trở lên
* Trình soạn thảo mã nguồn (Visual Studio Code)

### 5.2 Cài đặt thư viện

```bash
npm install
```

### 5.3 Chạy kiểm thử

```bash
npx cypress open
```

Sau đó chọn E2E Testing và chạy các file test trong thư mục `cypress/e2e`.

---

## 6. Kết quả

<img width="2564" height="1444" alt="Screenshot 2026-01-26 135314" src="https://github.com/user-attachments/assets/13fc8a97-5c14-479f-8f7a-23a5c4dee2b0" />

---<img width="2564" height="1444" alt="Screenshot 2026-01-26 135205" src="https://github.com/user-attachments/assets/21d2997b-0ac9-4007-8d6a-28e4dd5a956d" />

## 7. Ghi chú

* Website SauceDemo chỉ dùng cho mục đích học tập và thực hành kiểm thử.
* Không sử dụng cho môi trường thực tế.





