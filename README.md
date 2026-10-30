# Master Prompt Manager Pro

Ứng dụng desktop Windows quản lý thư viện Master Prompt, xây dựng bằng Tauri 2 + React + TypeScript và SQLite.

> Trạng thái: khởi tạo repository. Chưa phải bản phát hành ổn định; cần hoàn thiện, build và kiểm thử trước khi phát hành installer.

## Mục tiêu
- Quản lý Prompt, danh mục, tìm kiếm và yêu thích.
- Thay biến trong Prompt và xem trước nội dung.
- Lưu dữ liệu cục bộ bằng SQLite.
- Sao lưu/khôi phục JSON và quản lý lịch sử phiên bản.
- Tạo Windows NSIS `.exe` và MSI qua GitHub Actions.

## Build
Yêu cầu Node.js 20+ và Rust stable. Trên Windows runner, GitHub Actions sẽ cài WebView2/Tauri dependencies, build installer và đính kèm installer vào GitHub Release khi push tag `v*`.

## Trạng thái triển khai
Các tính năng và installer chỉ được coi là hoàn thành sau khi CI thành công và gói cài đặt được kiểm thử thực tế.