# In / Out Calorie PWA — Overwrite v13

Bản sửa lại từ đầu cho lỗi Calo Out.

## Thay đổi chính

- Đọc Google Sheet bằng CSV trước để giữ nguyên giá trị hiển thị ở cột C/D như `1h`, `5 mins`.
- Khóa cứng mapping Sheet: A ngày, B đồ ăn, C tập tạ, D cardio, E cân, F vòng eo.
- Tính lại Tổng calo ra = TDEE nền + calo tập tạ + calo cardio.
- Nếu cột C/D nhập trực tiếp `300 kcal`, web dùng trực tiếp số kcal đó.
- Lịch sử hiển thị rõ nguồn Sheet C/D để kiểm tra nhanh.
- Làm phần Ưu tiên số 1 trong Tổng quan to hơn, đậm hơn, rõ hơn.
- Cache Service Worker: `in-and-out-pwa-2026-07-11-v13`.

## Cách cập nhật

Giải nén ZIP, upload toàn bộ file vào thư mục gốc repository và chọn ghi đè file trùng tên.
Sau khi GitHub Pages cập nhật, đóng hẳn app/web rồi mở lại.
