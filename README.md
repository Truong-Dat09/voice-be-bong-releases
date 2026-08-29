# Voice_Bé_Bông v0.5.3

Phần mềm chuyển văn bản thành giọng nói chạy trên Windows.

## Ba file khách cần tải

Trong phần **Assets** của bản phát hành, tải đúng ba file:

1. `Voice_Bé_Bông_0.5.3_x64-setup.exe`
2. `Voice_Be_Bong_Offline_Public.cer`
3. `CAI_CHUNG_THU_OFFLINE.cmd`

Đặt cả ba file trong **cùng một thư mục**. Không đổi tên file `.cer` hoặc `.cmd`.

## Bước 1: Cài chứng thư công khai

1. Nhấp chuột phải `CAI_CHUNG_THU_OFFLINE.cmd`.
2. Chọn **Run as administrator / Chạy với quyền quản trị viên**.
3. Kiểm tra cửa sổ hiển thị Subject `CN=Voice_Be_Bong Offline`.
4. Nhập chính xác:

```text
DONG Y
```

5. Khi thấy thông báo thành công, khởi động lại Windows.

## Bước 2: Cài phần mềm

Sau khi Windows khởi động lại, chạy:

```text
Voice_Bé_Bông_0.5.3_x64-setup.exe
```

Hoàn tất trình cài đặt rồi mở **Voice_Bé_Bông** từ Desktop hoặc Start Menu.

## Model giọng nói

Model không được đóng gói sẵn trong bộ cài. Khách chọn engine/model nào thì phần mềm mới tải model đó. Model đã tải đầy đủ sẽ được dùng lại từ bộ nhớ đệm.

## Lưu ý bảo mật

- Chỉ cài chứng thư khi nhận file trực tiếp từ chủ sở hữu Voice_Bé_Bông.
- Chứng thư offline không được Smart App Control tin cậy như chứng thư Code Signing công cộng.
- Nếu Windows vẫn chặn tệp, không tắt bảo mật tùy tiện; hãy liên hệ chủ sở hữu để kiểm tra.
- Bản phát hành không chứa khóa updater riêng, mật khẩu, khóa kích hoạt khách hàng, `owner_tools` hoặc source riêng.

## Gỡ chứng thư khi không còn sử dụng

Mở `certlm.msc` bằng quyền Administrator và xóa chứng thư `Voice_Be_Bong Offline` tại:

- **Trusted Root Certification Authorities → Certificates**
- **Trusted Publishers → Certificates**
