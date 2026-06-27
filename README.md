# In and Out — GitHub Pages PWA

## Các file cần upload lên repository

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `README.md`

Upload các file vào **thư mục gốc** của nhánh `main`.

## Bật GitHub Pages

`Settings → Pages → Deploy from a branch → main → /(root) → Save`

## Cập nhật phiên bản sau này

Khi có HTML mới:

1. Đóng gói lại thành PWA.
2. Tăng tên `CACHE_NAME` trong `sw.js`.
3. Upload đè `index.html` và `sw.js`; nếu thay tên/icon thì upload thêm manifest và icon.
4. Chờ GitHub Pages triển khai lại, sau đó đóng hẳn app và mở lại.

## Quyền riêng tư

`index.html` đã có các thẻ `noindex`, `nofollow`, `noarchive`, `nosnippet`.
Điều này yêu cầu công cụ tìm kiếm không lập chỉ mục, nhưng không biến repository Public thành nội dung riêng tư.
