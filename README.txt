# 🏢 Hệ thống Quản lý Nhân viên (Employee Management System)


## 👋 Giới thiệu

Chào mừng bạn đến với **Hệ thống Quản lý Nhân viên**! Đây là một giải pháp hiện đại, mạnh mẽ được xây dựng trên nền tảng .NET mới nhất, giúp các doanh nghiệp số hóa và tối ưu hóa quy trình quản lý nhân sự một cách dễ dàng và bảo mật.

<p align="center">
  <strong>Gọn nhẹ — Bảo mật — Dễ sử dụng — Hiệu năng cao</strong>
</p>

---

## 📝 Mô tả dự án (Project Description)

Hệ thống Quản lý Nhân viên là giải pháp phần mềm tập trung nhằm tối ưu hóa việc quản trị dữ liệu nhân sự. Hệ thống hỗ trợ:

* 👤 **Quản lý hồ sơ:** Lưu trữ và cập nhật thông tin cá nhân nhân viên.
* 🔑 **Cấp phát tài khoản:** Tạo và quản lý thông tin đăng nhập.
* 🛡️ **Phân quyền (RBAC):** Gán vai trò và quyền truy cập chi tiết.
* 🔒 **Xác thực bảo mật:** Đảm bảo chỉ người dùng hợp lệ mới có thể truy cập hệ thống.

## 🚀 Công nghệ sử dụng (Tech Stack)

Dự án tự hào sử dụng các công nghệ tiên tiến:

* 🔷 **Framework:** .NET Core 9.0 (Hiệu năng vượt trội).
* 🗄️ **Database:** Microsoft SQL Server (Lưu trữ đáng tin cậy).
* 🔐 **Auth:** Cơ chế Xác thực & Phân quyền hệ thống tích hợp.
* 🛠️ **Tools:** SSMS, JSON Configuration, .NET CLI.

---

## 📸 Ảnh chụp màn hình (Screenshots)

*Hãy chèn ảnh chụp màn hình ứng dụng của Bình vào đây để người dùng dễ hình dung!*

<p align="center">
  <img src="https://via.placeholder.com/800x450.png?text=Bình+hãy+chèn+ảnh+chụp+màn+hình+vào+đây" alt="Placeholder ảnh" width="100%" />
</p>

---

## 🛠 Điều kiện tiên quyết (Prerequisites)

Trước khi bắt đầu, hãy đảm bảo máy bạn đã có:

* 🖥️ **.NET Core 9.0 SDK** (bản mới nhất).
* 🛢️ Phiên bản **Microsoft SQL Server**.
* 🛠️ **SQL Server Management Studio (SSMS)**.

---

## 🏗️ 1. Thiết lập Dự án (Project Setup)

### 1.1 Khôi phục Cơ sở dữ liệu 🔄

Hệ thống cần dữ liệu để hoạt động. Tệp sao lưu nằm trong thư mục **Database Folder**.

1.  Mở thư mục **Database Folder** và tìm tệp `.bak`.
2.  Mở **SSMS** và kết nối tới SQL Server.
3.  Chuột phải vào **Databases** -> chọn **Restore Database**.
4.  Chọn **Device**, tìm đến tệp `.bak`.
5.  Đặt tên cho CSDL và nhấn **OK**.

---

## ⚙️ 2. Cấu hình (Configuration)

### 2.1 Cấu hình Kết nối CSDL

Mở tệp `appsettings.json` ở thư mục gốc và cập nhật chuỗi kết nối:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=<TÊN_SERVER>;Database=<TÊN_CSDL>;User Id=<TÀI_KHOẢN>;Password=<MẬT_KHẨU>;"
  }
}
