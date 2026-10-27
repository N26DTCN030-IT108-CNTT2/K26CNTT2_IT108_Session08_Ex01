# Phần 1. Phân tích các lỗi cú pháp trong đoạn mã Markdown

Dưới đây là 3 lỗi chính xuất hiện trong đoạn bản thảo của bạn sinh viên khiến cho kết quả hiển thị trên StackEdit bị lỗi:

1. Lỗi phân cấp tiêu đề (Heading) bị nhảy cóc:
   - Hiện trạng: Đoạn mã sử dụng `# Lợi ích của rau sạch` (H1) nhưng ngay dòng bên dưới lại dùng `### Danh sách các loại rau` (H3).
   - Nguyên tắc & Hậu quả: Tiêu đề Markdown phải tuân thủ thứ tự phân cấp từ H1 đến H6 một cách tuần tự. Việc nhảy từ H1 xuống H3 làm mất tính logic của cấu trúc tài liệu, đồng thời trình soạn thảo không thể xác định đúng mối quan hệ cha - con giữa các mục.

2. Lỗi cú pháp chèn hình ảnh (Image):
   - Hiện trạng: Đoạn mã viết `[Logo Dự án] ( https://greentech.vn/logo.png )`.
   - Nguyên tắc & Hậu quả: Cú pháp chuẩn của ảnh trong Markdown là dấu chấm than đi trước cặp ngoặc vuông và ngoặc tròn liền mạch: `![Tên ảnh](đường_dẫn)`. Việc thiếu dấu chấm than `!` và để khoảng trắng ở các cặp dấu ngoặc khiến trình biên dịch hiểu nhầm đây là một đường dẫn liên kết (Link) thông thường thay vì tải và hiển thị hình ảnh.

3. Lỗi in đậm văn bản (Emphasis):
   - Hiện trạng: Đoạn mã viết `*Rất quan trọng`.
   - Nguyên tắc & Hậu quả: Để in đậm văn bản trong Markdown, ta phải dùng cặp dấu nhân đôi ở hai đầu là hai dấu sao `**văn bản**` hoặc hai dấu gạch dưới `__văn bản__`. Việc chỉ dùng một dấu sao đơn `*` sẽ khiến hệ thống hiểu đây là cú pháp tạo chữ nghiêng (Italic) hoặc khởi tạo danh sách, dẫn đến định dạng không đúng ý muốn.

---

# Phần 2. Hoàn thiện đoạn mã Markdown chuẩn

Dưới đây là đoạn mã Markdown đã được chỉnh sửa lại hoàn chỉnh, đúng cú pháp và bảo đảm phân cấp tiêu đề từ H1 đến H2:

![Rau Sạch](https://greentech.vn/logo.png)

# Lợi ích của rau sạch

## Danh sách các loại rau

**Rất quan trọng**
