# 20/10 — Những Bông Hoa Của 12A10 (bản không ảnh)

Website tĩnh chúc mừng 20/10 dành cho lớp 12A10. Bản này đã gỡ toàn bộ ảnh chụp, ảnh gallery, trình xem ảnh và tài nguyên hình ảnh. Hình minh họa ở đầu trang được tạo bằng CSS và ký tự trang trí, không dùng tệp ảnh. Tệp âm thanh `Chuyện rằng — Thịnh Suy` bạn cung cấp được giữ trong dự án.

## Tính năng

- Màn hình mở quà và giao diện pastel responsive.
- Phong thư tương tác và lá thư chúc mừng.
- Trình phát nhạc với phát/tạm dừng, thanh thời gian, tua bài, âm lượng và thông báo lỗi tải nhạc.
- Đủ 20 lời chúc cá nhân hóa; tìm kiếm và lọc theo chủ đề.
- Vườn 20 bông hoa tương tác.
- Bói vui tạo thông điệp ngẫu nhiên.
- Pháo hoa Canvas có nút bật/tắt, tự dừng và hỗ trợ giảm chuyển động.
- Không dùng ảnh raster, thẻ `<img>`, gallery hoặc lightbox.

## Cấu trúc thư mục

```text
lop12a10/
├── index.html
├── styles.css
├── script.js
├── README.md
├── .nojekyll
└── chuyen-rang.mp3
```

## Chạy thử

1. Giải nén ZIP.
2. Mở `index.html` bằng Chrome hoặc Edge.
3. Nhấn **Mở món quà 20/10**. Đây là thao tác của người dùng để trình duyệt cho phép bắt đầu phát nhạc.
4. Nếu nhạc không chạy khi mở tệp cục bộ, thử qua GitHub Pages hoặc chạy website bằng máy chủ cục bộ. Trình duyệt di động thường chặn autoplay nếu chưa có thao tác của người dùng.

## Cập nhật repository GitHub Pages hiện tại

1. Giải nén ZIP ra một thư mục.
2. Mở repository `lop12a10` trên GitHub.
3. Chọn **Add file → Upload files**.
4. Tải các tệp bên trong thư mục đã giải nén lên **thư mục gốc** của repository, bao gồm `index.html`, `styles.css`, `script.js`, `README.md`, `.nojekyll` và `chuyen-rang.mp3`.
5. Nếu GitHub hỏi ghi đè `index.html` hoặc `README.md`, chấp nhận để dùng bản mới. Đảm bảo `chuyen-rang.mp3` nằm cùng thư mục với `index.html`.
6. Nhấn **Commit changes**, đợi GitHub Pages triển khai lại rồi mở website và nhấn `Ctrl + F5`.

Đường dẫn nhạc phải đúng chính xác là `chuyen-rang.mp3`. Không tải riêng `index.html`, vì khi đó CSS, JavaScript và tệp nhạc sẽ thiếu.

## Trình phát nhạc

Âm thanh dùng HTML `<audio>` với tệp MP3 (`audio/mpeg`) được chuyển đổi từ tệp bạn cung cấp để tăng tính tương thích. Tệp đã được kiểm tra giải mã thành công và không kèm bìa ảnh nhúng. Đặt MP3 ngay ở thư mục gốc để tránh lỗi đường dẫn thư mục con. Nhạc không tự chạy ngay khi tải trang; nó được gọi sau khi người xem bấm mở quà hoặc nhấn nút phát. Khi đưa lên GitHub, hãy kiểm tra nhạc có phát được trên thiết bị thực tế hay không.

## Trạng thái bàn giao

- **Đã tạo:** bản website không ảnh và gói ZIP.
- **Đã kiểm tra tĩnh:** không còn thẻ `<img>`, không còn đường dẫn `gallery`, `lightbox` hoặc `og:image`; mã nguồn vẫn giữ nguyên danh sách 20 người và các tính năng tương tác không phụ thuộc ảnh.
- **Đã kiểm tra tệp nhạc:** tệp MP3 stereo 44.1 kHz, thời lượng khoảng 4 phút 37 giây; đã kiểm tra giải mã đầy đủ bằng FFmpeg.
- **Chưa xác minh trực tiếp trên GitHub Pages sau khi tải lên:** cần commit bản này vào repository và thử trên URL thực tế.


### Khắc phục nhanh khi nhạc không chạy
- Repository phải có tệp `chuyen-rang.mp3` ở thư mục gốc (chú ý chữ thường, dấu gạch ngang và phần mở rộng `.mp3`).
- Tải lên đồng thời `index.html`, `styles.css`, `script.js`, `.nojekyll`, `README.md` và `chuyen-rang.mp3`. Tất cả phải nằm cùng ở thư mục gốc; không tải nguyên file ZIP như một tệp trên GitHub.
- Sau khi nhấn **Commit changes**, mở website và nhấn `Ctrl + F5`. Nhạc chỉ bắt đầu sau khi người xem bấm nút mở quà hoặc nút phát.
- Nếu trình phát báo lỗi, liên kết `Mở tệp nhạc trực tiếp` sẽ hiện ra để kiểm tra tệp MP3 có được phục vụ bởi GitHub Pages hay không.
