# In / Out Calorie PWA — Overwrite v10

Gói cập nhật để upload đè lên repository GitHub Pages hiện tại.

## Sửa lỗi và nâng cấp

- Sửa phần Lịch sử calo In / Out: calo Out hiện cộng đúng TDEE nền + calo tập tạ + calo cardio.
- Đọc Google Sheet linh hoạt hơn: hỗ trợ nhận diện cột theo tiêu đề và mở rộng phạm vi từ A:F sang A:Z để tránh mất cột tập/cardio khi Sheet thay đổi thứ tự.
- Nhận diện thời lượng tập tốt hơn: hỗ trợ 60p, 60ph, 1h30, 1h30p, 01:30, 60 phút.
- Nếu ô tập/cardio nhập trực tiếp kcal, web dùng kcal đó làm calo tập.
- Khối “Ưu tiên số 1” ở Tổng quan được làm nổi bật hơn, số liệu kcal và thời gian đi bộ lớn, đậm và rõ hơn.
- Giữ logic ngày mai: chỉ hiện trong Lịch sử, chưa tính vào Tổng quan/Lịch năm/Biểu đồ/tổng lũy kế cho tới khi ngày đó tới.
- Cache Service Worker: `in-and-out-pwa-2026-07-11-v10`.

## Cách cập nhật

1. Giải nén ZIP.
2. Upload toàn bộ file bên trong vào thư mục gốc repository.
3. Chọn ghi đè các file trùng tên.
4. Chờ GitHub Pages cập nhật, sau đó đóng hẳn app/web và mở lại.
