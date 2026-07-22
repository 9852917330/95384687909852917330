# In / Out Calorie PWA — Overwrite v12

Gói cập nhật để upload đè lên repository GitHub Pages hiện tại.

## Sửa lỗi chính

- Sửa triệt để lỗi calo Out không cộng tập tạ/cardio trong Lịch sử.
- Cột C = Tập tạ, cột D = Cardio được đọc ưu tiên theo giá trị hiển thị của Google Sheets.
- Nhận đúng các dạng: `1h`, `1h30`, `1h 30p`, `01:30`, `5 mins`, `60 phút`, `[1,0,0,0]`, hoặc số duration của Google Sheets như `0.0416667`.
- Tổng calo ra trong Lịch sử = TDEE nền + calo tập tạ + calo cardio.
- Phần Ưu tiên số 1 ở Tổng quan được làm đậm, to và nổi bật hơn.
- Giữ logic ngày mai: chỉ hiển thị trong Lịch sử, chưa tính vào dashboard cho đến khi ngày đó tới.

## Cache

`in-and-out-pwa-2026-07-11-v12`

## Cách cập nhật

1. Giải nén ZIP.
2. Upload toàn bộ file vào thư mục gốc repo.
3. Chọn ghi đè file trùng tên.
4. Chờ GitHub Pages cập nhật, sau đó đóng hẳn app/web rồi mở lại.
