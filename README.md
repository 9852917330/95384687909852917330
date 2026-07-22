# In / Out Calorie PWA — Overwrite v11

Gói cập nhật để upload đè lên repository GitHub Pages hiện tại.

## Sửa lỗi chính

- Sửa lỗi Google Sheets trả ô thời gian `1h`/duration thành số thập phân ngày, làm web hiểu thành 0 phút.
- Cột C `Tập tạ` và cột D `Cardio` giờ đọc theo giá trị hiển thị của Sheet trước, sau đó mới dùng raw value.
- Parser thời gian nhận được: `1h`, `1h30`, `1:00`, `01:30`, `5 mins`, `60 phút`, số duration của Google Sheets như `0.0416667`.
- Lịch sử hiển thị rõ `Calo tập được cộng vào Out = tạ + cardio`.
- Khối Ưu tiên số 1 ở Tổng quan được làm đậm, lớn và nổi bật hơn.
- Cache Service Worker: `in-and-out-pwa-2026-07-11-v11`.

## Cách cập nhật

1. Giải nén ZIP.
2. Upload toàn bộ file bên trong vào thư mục gốc repository.
3. Chọn ghi đè file trùng tên.
4. Chờ GitHub Pages cập nhật, sau đó đóng hẳn app/web và mở lại.
