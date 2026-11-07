# Triết Quizz — Lý luận về Nhà nước

Trò chơi trắc nghiệm 6 câu hỏi Triết học Mác – Lênin, giữ nguyên câu hỏi/đáp án của file Word gốc. Giao diện responsive, hiệu ứng đúng/sai, âm thanh khi trình duyệt cho phép, bộ đếm số câu đã làm và số câu đúng. Thiết kế: **Design by Phan Huy x ChatGPT**.

## Chạy thử

Mở `index.html` bằng Chrome, Edge, hoặc Safari trên máy tính. Không cần cài Node.js, thư viện hay chạy server. Âm thanh có thể cần một lần chạm vào trang để trình duyệt cho phép phát.

## Đưa lên GitHub

1. Giải nén ZIP. **Không upload nguyên ZIP** nếu muốn GitHub/Render chạy trực tiếp; hãy upload **các file bên trong ZIP**.
2. Trên GitHub, tạo repository mới (ví dụ `triet-quizz`) tại https://github.com/new.
3. Vào repository > **Add file > Upload files**; chọn `index.html`, `render.yaml`, `README.md` trong thư mục vừa giải nén.
4. Chọn **Commit changes**. Kiểm tra `index.html` nằm ngay **thư mục gốc** của repository, không nằm trong thư mục con.

## Triển khai web bằng Render

1. Mở https://dashboard.render.com/ và đăng nhập / kết nối GitHub.
2. **New > Static Site** (không chọn Web Service).
3. Chọn repository `triet-quizz` vừa upload, nhánh `main`.
4. Cài đặt:
   - **Build Command:** `echo "Static HTML - no build required"`
   - **Publish Directory:** `.` (một dấu chấm, nghĩa là thư mục gốc)
5. Bấm **Create Static Site / Deploy Static Site**. Khi triển khai thành công, Render cung cấp địa chỉ dạng `https://ten-web.onrender.com` để chia sẻ.

Render có thể nhận file `render.yaml` nếu m dùng kiểu **New > Blueprint** thay vì tạo Static Site thủ công. Với cách thủ công trên, không cần cấu hình gì thêm.

## Cách khác: GitHub Pages

Trong repository > **Settings > Pages** > **Deploy from a branch** > `main` > `/(root)` > **Save**. GitHub Pages sẽ tạo đường dẫn trang web từ `index.html`.

## Lưu ý

- Toàn bộ CSS và JavaScript nằm trong `index.html`; không cần thêm thư viện hay tài nguyên bên ngoài.
- Website không có backend và không lưu lịch sử của người chơi trên server. Kết quả trên trang dùng để ôn tập.
- Sau này chỉnh `index.html` và commit lên GitHub, Render sẽ tự triển khai lại nếu bật Auto Deploy.
