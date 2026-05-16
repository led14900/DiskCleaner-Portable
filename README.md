# 🧹 Disk Cleaner

**Disk Cleaner** là ứng dụng dọn dẹp ổ đĩa (disk cleaner) dạng portable (không cần cài đặt) dành riêng cho Windows. Với **Disk Cleaner**, bạn có thể dễ dàng quét, xem xét và dọn dẹp các file rác, file tạm không cần thiết trên ổ cứng để lấy lại không gian lưu trữ quý giá. Là một công cụ disk cleaner thông minh, ứng dụng ưu tiên sự an toàn tuyệt đối: chỉ xóa các mục đã được quét, chặn tương tác với vùng hệ thống quan trọng và tự động cấp quyền Administrator để dọn dẹp triệt để nhất.

## 🚀 Tải bản mới nhất

**Bản ổn định hiện tại:** `v1.0.8`

📥 Tải trực tiếp:

- Bản portable không cần cài đặt: [Download DiskCleaner.exe](https://github.com/led14900/DiskCleaner-Portable/releases/download/v1.0.8/DiskCleaner.exe)
- Bản cài đặt Setup: [Download DiskCleanerSetup.exe](https://github.com/led14900/DiskCleaner-Portable/releases/download/v1.0.8/DiskCleanerSetup.exe)

Hoặc vào trang Releases:

[https://github.com/led14900/DiskCleaner-Portable/releases/latest](https://github.com/led14900/DiskCleaner-Portable/releases/latest)

## ⚙️ Cách chạy

1. Tải `DiskCleaner.exe` nếu muốn dùng bản portable, hoặc `DiskCleanerSetup.exe` nếu muốn cài đặt vào máy.
2. 🖱️ Chạy trực tiếp file đã tải.
3. 🛡️ Windows sẽ hỏi quyền Administrator qua UAC. Bấm `Yes` để cấp quyền cho phần mềm disk cleaner hoạt động với đầy đủ chức năng.

**⚠️ Lưu ý:** Do ứng dụng disk cleaner này chưa được đăng ký chứng chỉ số trả phí (chưa sign publisher), một số phiên bản Windows (như Windows Defender SmartScreen) có thể hiện cảnh báo bảo mật khi mở lần đầu. Bạn chỉ cần chọn **More info** -> **Run anyway** để sử dụng bình thường. Ứng dụng tự động yêu cầu quyền Administrator ngay khi mở để đảm bảo chức năng dọn rác hệ thống. Nếu bạn thấy popup hỏi quyền Administrator bên trong ứng dụng, hãy bấm `OK` để ứng dụng thử mở lại.

## ✨ Tính năng chính của Disk Cleaner

- 🗑️ **Quét file rác siêu tốc:** Dọn dẹp Windows Temp, cache trình duyệt, thumbnail cache, log, crash dump, prefetch, Windows Update cache, npm/yarn/pip cache...
- 💽 **Xử lý thư mục Windows.old:** Phần mềm disk cleaner hỗ trợ quét và dọn sạch sẽ thư mục `Windows.old` cứng đầu sau khi nâng cấp Windows.
- 📊 **Tìm file dung lượng lớn:** Quét và liệt kê các file lớn trên từng ổ đĩa để bạn tự do chọn lọc trước khi xóa.
- 👯 **Tìm file trùng lặp (Duplicate Finder):** So sánh và tìm file trùng lặp chính xác 100% bằng thuật toán mã băm SHA-256.
- ♻️ **Xóa an toàn:** Cho phép chuyển file vào Thùng rác hoặc xóa vĩnh viễn với các rào cản an toàn tích hợp.
- 📈 **Quản lý lịch sử:** Lưu lại lịch sử dọn dẹp, tổng dung lượng đã giải phóng và danh sách lỗi rõ ràng.
- 🇻🇳 **Giao diện thân thiện:** Giao diện 100% tiếng Việt, trực quan, dễ sử dụng cho mọi đối tượng.

## Lưu ý về Windows.old

Từ `v1.0.4`, `Windows.old` được xử lý riêng:

- Ứng dụng scan đúng thư mục `X:\Windows.old` theo ổ đĩa đang chọn.
- Khi dọn `Windows.old`, ứng dụng bỏ qua Thùng rác và dùng cơ chế xóa protected.
- Ứng dụng chỉ cho phép xóa đúng thư mục gốc `X:\Windows.old`, không mở quyền xóa tùy tiện các thư mục hệ thống khác.
- Cần chạy bằng quyền Administrator để xóa ổn định.

## 🔒 Cơ chế an toàn tuyệt đối

- 🧠 Disk Cleaner có lớp kiểm tra bảo vệ cuối cùng (Main process), không bao giờ tin tưởng tuyệt đối vào danh sách đường dẫn từ giao diện.
- ✅ Chỉ cho phép xóa các file/thư mục đã được công cụ quét disk cleaner xác nhận trong kết quả hiện tại.
- 🛑 Chặn tuyệt đối thư mục gốc ổ đĩa, thư mục Windows, Program Files, ProgramData, profile người dùng và các thư mục dữ liệu cá nhân quan trọng.
- 🔗 Chặn xử lý symlink, junction, shortcut liên kết và các đường dẫn không hợp lệ.
- ⚙️ Ngăn chặn xóa file thực thi hoặc file hệ thống như `.exe`, `.dll`, `.sys`, `.msi`, `.ps1`, `.reg`...
- 🛡️ Với file trùng lặp, phần mềm disk cleaner bắt buộc phải giữ lại ít nhất một bản gốc.

## 👨‍💻 Tác giả & Liên hệ

- **Tác giả:** `led14900`
- **SĐT / Zalo:** `0896009111`
- **GitHub:** [https://github.com/led14900](https://github.com/led14900)
- **Báo lỗi / Góp ý:** [https://github.com/led14900/DiskCleaner-Portable/issues](https://github.com/led14900/DiskCleaner-Portable/issues)

## 📄 Bản quyền

MIT License - Disk Cleaner (c) 2026 led14900
