# Portfolio cá nhân – Vũ Văn Tùng

## Giới thiệu

Website portfolio/CV cá nhân giới thiệu Vũ Văn Tùng, sinh viên Công nghệ Thông tin quan tâm đến phát triển web. Trang cung cấp phần giới thiệu, các kỹ năng, liên kết mạng xã hội và thông tin liên hệ. Giao diện được thiết kế responsive để sử dụng trên điện thoại, máy tính bảng và máy tính.

Đây là website tĩnh: không có backend, cơ sở dữ liệu, bước biên dịch hay gói phụ thuộc cần cài đặt.

## Chức năng

- Giới thiệu cá nhân và ảnh đại diện.
- Trình bày kỹ năng và sở thích.
- Hiển thị các thẻ liên kết đến Facebook và TikTok.
- Cung cấp thông tin liên hệ qua điện thoại và mạng xã hội.
- Điều hướng nhanh đến từng phần trong trang.
- Bố cục thích ứng nhiều kích thước màn hình.

## Công nghệ sử dụng

- **HTML5**: cấu trúc và nội dung trang.
- **CSS3**: giao diện, Flexbox, CSS Grid và bố cục responsive.
- **Tài nguyên tĩnh**: ảnh trong thư mục `assets/img/` và kiểu dáng trong `assets/css/styles.css`.

Trang không sử dụng JavaScript hoặc framework frontend.

## Yêu cầu môi trường

- Trình duyệt hiện đại như Chrome, Firefox, Edge hoặc Safari.
- Không cần cài Node.js, npm, cơ sở dữ liệu hay công cụ build.
- Git chỉ cần thiết nếu muốn tải mã nguồn bằng Git.
- Có thể dùng Python 3 để chạy máy chủ thử nghiệm cục bộ (không bắt buộc).
- Nếu chạy bằng Docker: cần cài Docker Desktop trên Windows/macOS hoặc Docker Engine trên Linux.
- Không cần biến môi trường, API key hay thông tin bí mật để chạy trang.
- Cần kết nối Internet để mở các liên kết mạng xã hội bên ngoài.

## Cấu trúc dự án

```text
.
├── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   └── img/
└── README.md
```

## Cài đặt và chạy thử

### Cách nhanh: mở trực tiếp

Tải hoặc giải nén dự án, sau đó mở `index.html` bằng trình duyệt. Không cần cài đặt thêm.

### Windows

Mở PowerShell tại thư mục dự án:

```powershell
Start-Process .\index.html
```

Hoặc chạy máy chủ thử nghiệm bằng Python 3:

```powershell
py -m http.server 8000
```

Mở <http://localhost:8000> trong trình duyệt. Nhấn `Ctrl+C` trong PowerShell để dừng máy chủ.

### macOS

Mở Terminal tại thư mục dự án:

```bash
open index.html
```

Hoặc chạy máy chủ thử nghiệm bằng Python 3:

```bash
python3 -m http.server 8000
```

Mở <http://localhost:8000> trong trình duyệt. Nhấn `Control+C` trong Terminal để dừng máy chủ.

### Linux

Mở Terminal tại thư mục dự án:

```bash
xdg-open index.html
```

Hoặc chạy máy chủ thử nghiệm bằng Python 3:

```bash
python3 -m http.server 8000
```

Mở <http://localhost:8000> trong trình duyệt. Nhấn `Ctrl+C` trong Terminal để dừng máy chủ.

> Máy chủ Python chỉ phục vụ thử nghiệm cục bộ, không nên dùng làm máy chủ triển khai production.

### Docker (Windows, macOS và Linux)

Cần khởi động Docker trước. Mở PowerShell hoặc Terminal tại thư mục chứa `index.html`, sau đó chạy lệnh tương ứng.

**Windows PowerShell:**

```powershell
docker run --rm -d --name portfolio-cv -p 8080:80 -v "${PWD}:/usr/share/nginx/html:ro" nginx:alpine
```

**macOS / Linux:**

```bash
docker run --rm -d --name portfolio-cv -p 8080:80 -v "$PWD:/usr/share/nginx/html:ro" nginx:alpine
```

Mở <http://localhost:8080> để xem trang. Dừng container bằng lệnh:

```bash
docker stop portfolio-cv
```

Lệnh Docker sử dụng Nginx từ image `nginx:alpine` và mount thư mục dự án ở chế độ chỉ đọc; không cần tạo Dockerfile hoặc build image riêng. Nếu cổng `8080` đang được sử dụng, thay `8080` ở phía trái của `-p` bằng một cổng khác và truy cập đúng cổng đó.

## Cấu hình và tùy chỉnh

Website không có tệp cấu hình môi trường. Để cập nhật nội dung:

- Sửa thông tin, phần giới thiệu, các liên kết và nội dung trang trong `index.html`.
- Thay ảnh trong `assets/img/` hoặc cập nhật đường dẫn ảnh tương ứng trong `index.html`.
- Chỉnh màu sắc, bố cục và giao diện trong `assets/css/styles.css`.
- Sau khi thay đổi, tải lại trang trong trình duyệt để xem kết quả.

## Thông tin liên hệ

- **Người thực hiện:** Vũ Văn Tùng
- **Điện thoại:** [0922757015](tel:0922757015)
- **Facebook:** [facebook.com/vuthanhtungdeptrai.08](https://www.facebook.com/vuthanhtungdeptrai.08)
- **TikTok:** [@tungtkt](https://www.tiktok.com/@tungtkt)