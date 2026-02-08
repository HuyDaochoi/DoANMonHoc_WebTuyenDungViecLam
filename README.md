# REQUIREMENT DỰ ÁN WEBSITE TUYỂN DỤNG VIỆC LÀM

## 1. Thông tin chung

* **Tên dự án:** Website Tuyển Dụng Việc Làm
* **Mục tiêu:** Xây dựng website hỗ trợ kết nối giữa **Nhà tuyển dụng** và **Ứng viên**, cho phép đăng tin tuyển dụng, tìm kiếm việc làm và nộp hồ sơ trực tuyến.
* **Đối tượng sử dụng:**

  * Khách truy cập (Guest)
  * Ứng viên (Candidate)
  * Nhà tuyển dụng (Employer)
  * Quản trị viên (Admin)

---

## 2. Công nghệ sử dụng

* **Backend:** Node.js, Express.js
* **Cơ sở dữ liệu:** MySQL (chạy trên Laragon)
* **Quản lý CSDL:** HeidiSQL
* **Frontend:** HTML, CSS, JavaScript (có thể mở rộng React/Vue nếu cần)
* **Mô hình kiến trúc:** MVC (Model – View – Controller)

---

## 3. Phạm vi dự án

Dự án tập trung vào các chức năng cốt lõi của một website tuyển dụng ở mức **đồ án môn học**, không yêu cầu thanh toán trực tuyến hay AI gợi ý nâng cao.

---

## 4. Chức năng hệ thống

### 4.1. Chức năng cho Khách truy cập (Guest)

* Xem danh sách việc làm
* Tìm kiếm việc làm theo:

  * Tên công việc
  * Địa điểm
  * Mức lương
* Xem chi tiết tin tuyển dụng
* Đăng ký tài khoản Ứng viên / Nhà tuyển dụng
* Đăng nhập hệ thống

---

### 4.2. Chức năng cho Ứng viên (Candidate)

* Quản lý tài khoản cá nhân
* Cập nhật hồ sơ cá nhân (CV):

  * Thông tin cá nhân
  * Kỹ năng
  * Kinh nghiệm làm việc
* Tìm kiếm và xem chi tiết việc làm
* Nộp hồ sơ ứng tuyển cho công việc
* Xem danh sách công việc đã ứng tuyển
* Hủy ứng tuyển (nếu chưa được duyệt)

---

### 4.3. Chức năng cho Nhà tuyển dụng (Employer)

* Quản lý thông tin công ty
* Đăng tin tuyển dụng
* Chỉnh sửa / xóa tin tuyển dụng
* Xem danh sách ứng viên ứng tuyển
* Duyệt hoặc từ chối hồ sơ ứng viên

---

### 4.4. Chức năng cho Quản trị viên (Admin)

* Đăng nhập trang quản trị
* Quản lý tài khoản người dùng
* Quản lý tin tuyển dụng
* Khóa / mở khóa tài khoản vi phạm
* Thống kê cơ bản:

  * Số lượng người dùng
  * Số lượng tin tuyển dụng
  * Số lượng hồ sơ ứng tuyển

---

## 5. Yêu cầu chức năng chi tiết (Functional Requirements)

### FR-01: Đăng ký tài khoản

* Người dùng có thể đăng ký với email và mật khẩu
* Chọn loại tài khoản: Ứng viên hoặc Nhà tuyển dụng

### FR-02: Đăng nhập

* Xác thực email và mật khẩu
* Phân quyền theo vai trò người dùng

### FR-03: Quản lý tin tuyển dụng

* Nhà tuyển dụng có thể tạo, sửa, xóa tin tuyển dụng
* Tin tuyển dụng gồm: tiêu đề, mô tả, yêu cầu, mức lương, địa điểm

### FR-04: Ứng tuyển việc làm

* Ứng viên có thể nộp hồ sơ cho một công việc
* Mỗi công việc chỉ được ứng tuyển một lần

---

## 6. Yêu cầu phi chức năng (Non-Functional Requirements)

* Hệ thống phản hồi trong vòng < 3 giây
* Bảo mật mật khẩu bằng mã hóa
* Giao diện thân thiện, dễ sử dụng
* Code rõ ràng, dễ bảo trì
* Có khả năng mở rộng trong tương lai

---

## 7. Yêu cầu cơ sở dữ liệu (Database Requirements)

### Các bảng chính:

* users
* companies
* jobs
* applications
* roles

### Quan hệ dữ liệu:

* Một nhà tuyển dụng có nhiều tin tuyển dụng
* Một tin tuyển dụng có nhiều hồ sơ ứng tuyển
* Một ứng viên có thể ứng tuyển nhiều công việc

---

## 8. Use Case tổng quát

* UC01: Đăng ký tài khoản
* UC02: Đăng nhập hệ thống
* UC03: Đăng tin tuyển dụng
* UC04: Tìm kiếm việc làm
* UC05: Ứng tuyển việc làm
* UC06: Quản lý người dùng (Admin)

---

## 9. Định hướng mở rộng

* Upload CV dạng PDF
* Gửi email thông báo khi có ứng tuyển
* Phân trang và lọc nâng cao
* Thống kê biểu đồ

---

## 10. Kết luận

Dự án Website Tuyển Dụng Việc Làm đáp ứng đầy đủ các yêu cầu cơ bản của một hệ thống tuyển dụng trực tuyến, phù hợp cho đồ án cuối môn học lập trình web với công nghệ Node.js và MySQL.
