# In and Out — GitHub Pages PWA V6

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


## Cập nhật 10/07/2026
- Bổ sung Protein, Carb và Fat cho từng món theo đúng khẩu phần đã nhận diện.
- Ba chất được tự động sắp xếp từ số gram cao nhất đến thấp nhất.
- Bổ sung tổng macro theo ngày và nâng cache Service Worker lên v5.


## Cập nhật 11/07/2026 — sửa hệ thống calo và macro
- Tách riêng **đậu hũ non** khỏi đậu phụ thường; dùng hồ sơ dinh dưỡng theo 100 g.
- Tách riêng **sữa bột tách béo / skim milk powder** khỏi sữa tách béo dạng lỏng.
- Đồng bộ calo, Protein, Carb và Fat từ cùng một hồ sơ cho các nguyên liệu chính.
- Sửa lỗi dữ liệu `null` bị hiểu nhầm thành 0 ở món tra trực tuyến.
- Bỏ việc âm thầm áp mặc định 200 kcal/100 g hoặc 60 kcal/100 ml khi đã có thể quy đổi từ khẩu phần/macro.
- Thêm kiểm tra chéo năng lượng `Protein×4 + Carb×4 + Fat×9`; tự cảnh báo hoặc hiệu chỉnh khi sai lệch lớn.
- Cập nhật Service Worker lên cache **v6** để PWA nhận bản sửa mới.


## Cập nhật V6 — CSDL món thường ăn và cách chế biến
- Bổ sung **188 hồ sơ ưu tiên**, có tên tiếng Việt, tên tiếng Anh và alias không dấu.
- Các món hoàn chỉnh có khẩu phần tham chiếu; nguyên liệu có dữ liệu theo 100 g/100 ml.
- Nhận diện và tự cộng phần dầu/sốt ước tính cho: **xào, chiên, rán, quay, nướng, trộn**.
- Với **luộc, hấp, hầm, tần**, hệ thống không tự cộng dầu.
- Nếu món đã là công thức hoàn chỉnh (ví dụ gà rán KFC, ngan cháy tỏi, cá kho), hệ thống không cộng chế biến lần hai.
- Tăng cache Service Worker lên **v7**.

> Món nhà hàng vẫn có sai số do khẩu phần, lượng dầu, da/mỡ, nước sốt và topping. Nhập khối lượng thực tế sẽ chính xác hơn nhập tên món đơn thuần.
