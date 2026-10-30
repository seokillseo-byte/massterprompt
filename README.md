# Master Prompt Manager Pro

Ứng dụng desktop Windows quản lý thư viện Master Prompt, xây dựng bằng Tauri 2 + React + TypeScript và SQLite.

## Trạng thái hiện tại

Đây là bản khởi tạo đang được kiểm tra trên GitHub Actions. Chưa phát hành installer ổn định và chưa được kiểm thử trên máy Windows người dùng.

## Chức năng đã có trong mã nguồn

- Thêm, sửa, xóa Master Prompt.
- Phân loại, tìm kiếm và đánh dấu yêu thích.
- Tự nhận diện biến `[Tên biến]` và `<<Tên biến>>`.
- Nhập giá trị biến, xem trước và sao chép Prompt.
- Sao lưu và nhập thư viện Prompt bằng JSON.
- Lưu Prompt và lịch sử phiên bản trong SQLite.
- Khôi phục phiên bản Prompt.

## Công nghệ

- Tauri 2 / Rust
- React / TypeScript / Vite
- SQLite qua `@tauri-apps/plugin-sql`

## Build tự động

Workflow `.github/workflows/release.yml` chạy build Windows khi có push lên nhánh `main` hoặc tag `v*`. Khi build từ tag, workflow đính kèm các gói NSIS `.exe` và MSI vào GitHub Release.

## Các phần còn cần hoàn thiện

- Workflow Builder và lưu workflow bằng SQLite.
- Kiểm thử import/export dữ liệu, lịch sử phiên bản và khôi phục trên Windows.
- Bổ sung icon ứng dụng và hoàn thiện giao diện.
- Chạy CI thành công, kiểm thử installer rồi mới phát hành bản tải chính thức.

## Lưu ý

Không xem bản mã nguồn hiện tại là sản phẩm hoàn thiện. Chỉ thông báo có file cài đặt khi GitHub Actions đã tạo gói thành công và Release có asset tải được.
