# THIẾT KẾ HỆ THỐNG ĐA PROFILE CAREPULSE

## PHẦN 1: PHÂN TÍCH ĐA PROFILE

**1. Nguyên nhân Session Conflict**

Dùng chung một Chrome Profile khiến Cookies và phiên đăng nhập bị dùng chung. Khi người khác đăng nhập tài khoản mới, phiên cũ có thể bị ghi đè và tự động đăng xuất.

**2. Thiết kế 3 Profile**

| Profile | Mục đích | Màu |
|---|---|---|
| Work | Công việc CarePulse | Xanh dương |
| Personal | Tài khoản cá nhân | Xanh lá |
| Sandbox/Test | Thử nghiệm website | Cam |

Mỗi Profile có Cookies, History, Bookmarks và Extensions riêng biệt.

## PHẦN 2: BOOKMARK VÀ AN TOÀN

**3. Cấu trúc Bookmark**

- **01_CarePulse_Clinic:** CarePulse, Cổng BHYT, Bộ Y tế.
- **02_Pharma_Portal:** Dược thư Quốc gia, Cục Quản lý Dược, Tra cứu thuốc.
- **03_Medical_Tools:** Google Dịch, Google Scholar, PubMed.

**4. Favicon-Only**

Nhấn chuột phải vào Bookmark → Chỉnh sửa → Xóa tên trang web, chỉ giữ biểu tượng → Lưu.

Áp dụng cho CarePulse, Cổng BHYT, Dược thư và Google Dịch để tiết kiệm diện tích thanh Bookmark.

**5. Xử lý an ninh**

Nên sử dụng **Guest Profile** khi cho khách mượn máy vì dữ liệu duyệt web của khách sẽ bị xóa khi kết thúc phiên.

Không nên dùng Incognito thay thế Guest Profile hoặc bật Cloud Sync tài khoản cá nhân vì có nguy cơ lộ mật khẩu, lịch sử và dữ liệu riêng tư.
