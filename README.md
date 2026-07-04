# In and Out — GitHub Pages PWA V4

## Bộ file upload lên repository

Upload đè toàn bộ file trong ZIP vào thư mục gốc của nhánh `main`:

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `README.md`

## Bản V4 đã nâng cấp

- Tăng CSDL nội bộ món Việt + món Tây thêm 136 mục V4.
- Ưu tiên nhận diện món Việt, món Tây, alias tiếng Việt không dấu và tiếng Anh.
- Thứ tự tra món: Local V4 → USDA FoodData Central → Open Food Facts.
- Open Food Facts dùng cho đồ đóng gói/barcode/sản phẩm siêu thị.
- Tăng phiên bản cache Service Worker để điện thoại nhận bản mới.
- Giữ `noindex`, `nofollow`, `noarchive`, `nosnippet`.

## Bật GitHub Pages

`Settings → Pages → Deploy from a branch → main → /(root) → Save`

## Cập nhật sau khi upload

Sau khi GitHub Pages build xong, mở app trên điện thoại, đóng hẳn app cũ rồi mở lại. Nếu vẫn chưa nhận bản mới, vào trình duyệt xóa dữ liệu website hoặc uninstall PWA cũ rồi cài lại.

## Lưu ý dữ liệu dinh dưỡng

Các món không có trọng lượng cụ thể vẫn là ước tính theo khẩu phần chuẩn. Muốn chính xác hơn, nhập kiểu: `ức gà 200g`, `cơm 150g`, `latte 300ml`, hoặc nhập trực tiếp `450 kcal`.
