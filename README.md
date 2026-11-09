# 6551071078_MAP_WEB

Võ Hồng Thiên - 6551071078 - CQ.65.CNTT

## Quản lý hoạt động khách sạn (HotelManagement) - LAB 3

Ứng dụng WinForms (.NET 8, C#) + Entity Framework Core + SQL Server. Project đầy đủ, mở là build và chạy được.

**Nội dung LAB 3 (theo "Tài liệu lab 3"):**
1. Quản lý dịch vụ khách dùng khi đang thuê phòng (`PhieuThue/FormThemDichVuPhongDaDung`, `FormDanhSachDichVuPhongDaDung`).
2. Quản lý phiếu đặt/thuê phòng: danh sách, tìm kiếm, xuất Excel, chi tiết phiếu, huỷ, cập nhật trạng thái, thanh toán (`PhieuThue/`). Menu "Danh sách đặt phòng".
3. Quản lý hoá đơn: danh sách, lọc theo ngày, tìm kiếm, xuất Excel, xem và in hoá đơn PDF (`HoaDon/`). Menu "Danh sách hóa đơn".
4. Quản lý tài khoản và quyền: danh sách, tìm kiếm, xuất Excel, thêm / sửa / xoá (`TaiKhoan/`). Menu "Danh sách tài khoản".
5. Dashboard thống kê kinh doanh theo khoảng thời gian (`ThongKe/FormThongKe`, biểu đồ `WinForms.DataVisualization`). Menu "Thống kê".

**Chạy thử**
1. Chạy `Database/Database.sql` trong SQL Server (SSMS), hoặc `sqlcmd -I -i Database/Database.sql`.
   CSDL tạo từ bản cũ thì chạy thêm `Database/NangCap_MaHD_10KyTu.sql` (mã hoá đơn dài 10 ký tự).
2. Đổi `ConnectionString` trong `Models/HotelManagementContext.custom.cs` cho đúng máy (mặc định `(localdb)\MSSQLLocalDB`).
3. Mở `HotelManagement.slnx` bằng Visual Studio 2022 và chạy. Tài khoản mẫu: `admin` / `1234`.

**Unit test:** `dotnet test HotelManagement.Tests` (test có dùng CSDL tự bỏ qua nếu không kết nối được; test ghi dữ liệu tự tạo và tự xoá dữ liệu tạm).
