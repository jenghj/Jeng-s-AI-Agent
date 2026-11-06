# Agent Tổng hợp Nội dung

Trang trưng bày tĩnh cho Hermes profile `lark-academic-coordinator`. Trang giới thiệu vai trò, năng lực, quy trình, quy tắc phán đoán, ranh giới, cách sử dụng và trạng thái cấu hình Lark.

## Mở trang

Mở `index.html` trong trình duyệt. Nút `VI / 中文` chuyển ngôn ngữ; phần demo dùng dữ liệu giả lập trong `demo.js` và hiển thị ngay trong trình duyệt.

## Thiết kế

- Giao diện hiện đại với bảng màu xanh trời, xanh dương và điểm nhấn xanh mint.
- Minh họa quỹ đạo chuyển động khoảng 290px trên nền gradient xanh đêm; các khối nền sáng dùng chữ đen và các khối nền tối dùng chữ trắng.
- Nội dung dùng Be Vietnam Pro, câu trích dẫn dùng Lora. Font cùng giấy phép được lưu trong assets/fonts; đã kiểm tra bộ ký tự tiếng Việt. Tiếng Trung dùng Microsoft YaHei/PingFang/Noto Sans SC làm font dự phòng.
- Bố cục co giãn cho máy tính và điện thoại; hỗ trợ giảm chuyển động. Đã xem bản chụp hiển thị trên Edge ở kích thước desktop và điện thoại.
- Các câu trích dẫn được biên soạn riêng cho trang, không gán cho tác giả bên ngoài.

## Trạng thái kết nối

- Hermes gateway đã được khởi động lại.
- Cấu hình định tuyến platform `feishu` tới profile `lark-academic-coordinator` đã được lưu.
- Cần một lượt nhắn thử trên Lark để xác nhận phản hồi sau khi định tuyến.

## Riêng tư và triển khai

- Website không chứa thông tin xác thực, token, dữ liệu chat thật hay thông tin nguồn riêng.
- Trang demo không gửi yêu cầu tới Hermes/Lark, không tải tệp lên và không có backend.
- Có thể triển khai như static site; không bật Functions/Worker hoặc thêm API nếu muốn giữ nguyên ranh giới riêng tư.
