# Trang chọn lớp học → link tương ứng

Web tĩnh (HTML/CSS/JS), chạy miễn phí trên **GitHub Pages**.

- `index.html` – trang cho học sinh
- `admin.html` – trang quản trị: sửa mọi link, thêm/xóa Level, cấp học, mật khẩu...
- `data.js` – nơi lưu toàn bộ nội dung (trang quản trị sẽ tự ghi file này)

## Đưa lên GitHub (1 lần)
1. Vào https://github.com/new → đặt tên repo (vd `hoc-tap`) → **Public** → Create.
2. Bấm **uploading an existing file**, kéo thả TOÀN BỘ file trong thư mục này (kể cả `.nojekyll`) → Commit.
3. **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save.**
4. Sau ~1 phút, link công khai: `https://TÊN_TÀI_KHOẢN.github.io/TÊN_REPO/`
   Trang quản trị: `.../admin.html`

## Cho phép trang quản trị lưu thay đổi
1. GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens → Generate new token**.
2. Repository access: **Only select repositories** → chọn repo này.
3. Permissions → Repository permissions → **Contents: Read and write** → Generate, copy token.
4. Mở `admin.html`, dán token (owner/repo tự nhận), sửa link, bấm **Lưu lên GitHub**. Đợi 1–2 phút để web cập nhật.

Chỉ người có token mới lưu được; học sinh mở admin.html cũng không sửa được gì.
Nếu không muốn dùng token: bấm **Tải data.js**, rồi upload đè file `data.js` trong repo.
