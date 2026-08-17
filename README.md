# Template Báo cáo thực tập (Hugo)

Dự án này là trang web báo cáo thực tập mẫu được xây dựng bằng **Hugo Static Site Generator** và sử dụng theme **Learn**. Bạn có thể sử dụng dự án này như một template để tạo báo cáo thực tập hoặc tài liệu cá nhân của riêng mình.

---

## 🛠️ Yêu cầu hệ thống

Trước khi bắt đầu, hãy cài đặt các công cụ sau trên máy tính của bạn:
1.  **Hugo Extended**: Hãy tải bản **Extended** (để biên dịch các file style Sass/SCSS của theme).
    *   Tải về từ: [Hugo Releases](https://github.com/gohugoio/hugo/releases)
    *   Hướng dẫn nhanh (cho Windows): Tải file zip `hugo_extended_..._windows-amd64.zip`, giải nén và thêm đường dẫn thư mục chứa file `hugo.exe` vào biến môi trường `PATH`.
2.  **Git**: Dùng để quản lý mã nguồn và đẩy dự án lên GitHub.

---

## 🚀 Hướng dẫn chạy thử cục bộ (Local Preview)

Mở Terminal hoặc PowerShell tại thư mục dự án và chạy các lệnh sau:

1.  **Khởi chạy Server chạy thử:**
    ```bash
    hugo server -D
    ```
    *Lưu ý: Tham số `-D` giúp hiển thị cả các bài viết nháp (draft: true).*

2.  **Xem kết quả:**
    Mở trình duyệt và truy cập: [http://localhost:1313](http://localhost:1313)
    *Khi bạn chỉnh sửa bất kỳ file Markdown hay cấu hình nào, trang web sẽ tự động làm mới.*

3.  **Biên dịch (Build) thủ công:**
    Để xuất ra các file tĩnh chuẩn bị đưa lên hosting khác:
    ```bash
    hugo --minify
    ```
    *Thư mục đầu ra sẽ là `public/`.*

---

## 📝 Hướng dẫn cá nhân hóa Template

### 1. Cấu hình thông tin trang web
Mở file `config.toml` ở thư mục gốc:
*   `baseURL`: Đổi thành địa chỉ web của bạn trên GitHub Pages (Ví dụ: `https://<ten-user>.github.io/<ten-repo>/`).
*   `author`: Thay đổi email của bạn.
*   Thay đổi tiêu đề trang web (`title`) trong phần `[Languages.en]` (Tiếng Anh) và `[Languages.vi]` (Tiếng Việt).
*   Chỉnh sửa hoặc xóa các link shortcuts (`[[Languages.en.menu.shortcuts]]`) ở thanh menu bên trái.

### 2. Thông tin cá nhân tại Trang chủ
Chỉnh sửa thông tin cá nhân của bạn trong các file sau:
*   Tiếng Việt: `content/_index.vi.md`
*   Tiếng Anh: `content/_index.md`

**Thay đổi ảnh đại diện:**
*   Chuẩn bị ảnh chân dung của bạn và lưu đè vào file `static/images/MyProfile.png` (giữ nguyên tên file). Hoặc bạn có thể thêm ảnh khác vào thư mục `static/images/` và thay đổi đường dẫn ảnh trong 2 file `_index` ở trên.

### 3. Cách thêm nội dung & bài viết mới

Hugo sắp xếp các mục bằng thuộc tính `weight` trong phần đầu của mỗi file markdown (**Front Matter**):
```yaml
---
title: "Tên bài viết hoặc tiêu đề tuần"
weight: 1            # Thứ tự hiển thị ở menu bên trái (số nhỏ hơn xếp trước)
chapter: false       # true nếu đây là tiêu đề chương lớn (không chứa nội dung chi tiết trực tiếp)
---
```

*   **Chuyên mục lớn (ví dụ: Worklog, Proposal, Workshop):** Mỗi mục lớn là một thư mục trong `content/` và phải chứa file `_index.md` (English) và `_index.vi.md` (Vietnamese).
*   **Bài viết con (ví dụ: Nhật ký ngày, bài viết con):** Đặt trong thư mục con tương ứng, mỗi bài viết con cũng cần có các file markdown đa ngôn ngữ tương ứng.
*   **Hình ảnh đính kèm**: Lưu hình ảnh vào thư mục `static/images/` và tham chiếu đến chúng trong file markdown bằng đường dẫn tuyệt đối bắt đầu từ root (ví dụ: `/images/ten-anh.png`).

---

## 🌐 Triển khai lên GitHub Pages (Tự động)

Dự án này đã được cấu hình sẵn **GitHub Actions** tại file `.github/workflows/hugo.yml` giúp tự động xây dựng và xuất bản trang web khi bạn đẩy code lên GitHub.

Các bước thực hiện:
1.  Tạo một repository mới trên GitHub và đẩy toàn bộ mã nguồn này lên nhánh `master` (hoặc đổi nhánh trong file workflow nếu cần).
2.  Truy cập vào Repository của bạn trên GitHub -> **Settings** -> **Pages**.
3.  Tại phần **Build and deployment** -> **Source**, chọn **GitHub Actions**.
4.  Khi đẩy mã nguồn lên nhánh `master`, tab **Actions** sẽ chạy quá trình build tự động. Sau khi hoàn thành, trang web của bạn sẽ hiển thị tại đường dẫn ở mục **GitHub Pages**.
