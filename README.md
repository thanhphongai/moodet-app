# Moodet landing page

Trang giới thiệu tĩnh cho ứng dụng Moodet. Một file `index.html` + thư mục `img/`, không cần build.

## Đưa lên GitHub Pages
1. Tạo repo trên GitHub (ví dụ `moodet-app`), đẩy toàn bộ thư mục này lên nhánh `main`.
2. Vào Settings → Pages → Source: Deploy from a branch → Branch `main`, folder `/ (root)` → Save.
3. Vài phút sau trang chạy ở `https://<user>.github.io/moodet-app/`.
4. Muốn dùng tên miền riêng: thêm file `CNAME` chứa tên miền (ví dụ `moodet.app`), trỏ DNS theo hướng dẫn của GitHub Pages, rồi bật Enforce HTTPS.

Sau khi có tên miền, sửa `og:image` trong `index.html` thành URL tuyệt đối (ví dụ `https://moodet.app/img/post.jpg`) để ảnh xem trước hiện đúng khi chia sẻ.

## Ghi chú
- Song ngữ VI/EN; mặc định chế độ sáng, người xem có thể chuyển tối, lựa chọn nhớ bằng localStorage.
- `img/logo.png` là logo app (dùng cho nav, footer, favicon, ảnh OG).
- Font Coiny, Baloo 2, Pacifico tải từ Google Fonts.
- Ảnh trong `img/` từ Wikimedia Commons (CC0 / public domain).
- `.nojekyll` để GitHub Pages không chạy Jekyll.
- Các link canonical, og:url, og:image trong `index.html` đang trỏ tới `https://thanhphongai.github.io/moodet-app/`; nếu sau này gắn tên miền riêng thì thay bằng tên miền đó.
