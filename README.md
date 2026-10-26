# Hành vi khách hàng · Study Studio

Website học tập bằng tiếng Việt theo bài giảng **HÀNH VI KH-HK3-2026 – Full** gồm 302 slide, 7 chương. Mục tiêu: hiểu khái niệm, phân tích hành vi mua và vận dụng vào các quyết định marketing.

**[Mở website học tập](https://datmoitapdev.github.io/hanh-vi-khach-hang-study/)**

## Nội dung

1. Tổng quan về hành vi khách hàng.
2. Các yếu tố bên ngoài: văn hóa, xã hội và tình huống.
3. Các yếu tố tâm lý: nhu cầu, động cơ, nhận thức, học hỏi và thái độ.
4. Các yếu tố cá nhân.
5. Quy trình ra quyết định mua của khách hàng cá nhân.
6. Hành vi mua của khách hàng tổ chức.
7. Quy trình ra quyết định mua của khách hàng tổ chức.

## Tính năng

- 37 bài học có diễn giải, ví dụ và điểm dễ nhầm.
- 42 câu trắc nghiệm kèm lời giải và số slide đối chiếu; luyện theo chương, tự kiểm tra và ôn câu sai.
- 37 flashcard và 7 tình huống tự luận có gợi ý, tiêu chí tự đánh giá.
- 5 công cụ thực hành: hành trình cá nhân, quy trình B2B, chấm nhà cung cấp, thay đổi tương đối và phân loại tình huống.
- Tra cứu văn bản, bảng và hình từ bài giảng; tải file PowerPoint gốc.
- Ghi chú, lưu tiến độ trên trình duyệt, nhập/xuất tiến độ JSON và in phiếu thực hành.
- Giao diện phù hợp máy tính và điện thoại; không cần cài thư viện ngoài.

## Chạy trên Windows

Cài Python, mở Terminal trong thư mục dự án và chạy:

```bash
py -m http.server 8080 --directory dist
```

Mở `http://localhost:8080`. Trên hệ thống khác có thể dùng `python` hoặc `python3` thay cho `py`.

## Đăng bằng GitHub Pages

GitHub Pages đã được cấu hình dùng **GitHub Actions** với workflow `.github/workflows/pages.yml`. Workflow triển khai thư mục `dist` sau mỗi lần đẩy lên `main`; có thể chạy thủ công tại tab **Actions**.

## Cấu trúc

- `dist/index.html`, `dist/style.css`, `dist/app.js`: giao diện và chức năng.
- `dist/lessons.json`, `dist/quiz.json`: bài học và ngân hàng câu hỏi.
- `dist/slides.json`, `dist/assets/`, `dist/bai-giang-goc.pptx`: tài liệu đối chiếu.
- `build_content.py`, `make_quiz.py`: tạo lại dữ liệu bài học và câu hỏi; chạy từ thư mục gốc.

Ví dụ và bài luyện được biên soạn thêm để học, không phải đề thi chính thức. Sơ đồ tạo bằng các đối tượng PowerPoint cần được xem trong file gốc để giữ đúng bố cục. Nội dung bài giảng thuộc tác giả tương ứng. Ghi chú và tiến độ chỉ được lưu trên trình duyệt, không tự đồng bộ giữa thiết bị.
