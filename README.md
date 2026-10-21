# Viên Minh Các — Lập lá số Tâm Số Học

Bản mẫu website tĩnh để bắt đầu xây dựng công cụ lập lá số theo hệ thống riêng của Viên Minh Các.

## Có trong bản mẫu
- Nhập thông tin người lập lá số.
- Nhập dữ liệu cho 12 cung: tên cung, Tâm số/số liệu, chính tinh/phụ tinh, yếu tố bổ sung, luận giải.
- Lưu hồ sơ trong trình duyệt hiện tại (localStorage).
- Xuất/nhập hồ sơ JSON.
- In báo cáo hoặc lưu thành PDF từ trình duyệt.
- Giao diện tương thích màn hình máy tính và điện thoại.

## Quan trọng
Bản mẫu **chưa tự tính lá số và chưa tự sinh luận giải**. Chúng tôi không tự giả định công thức riêng của Viên Minh Các. Các công thức và quy tắc sẽ được triển khai sau khi chủ hệ thống cung cấp và xác nhận tài liệu.

## Đưa website lên GitHub Pages
1. Tạo repository công khai mới trên GitHub, ví dụ `vien-minh-cac-tam-so-hoc`.
2. Tải `index.html` lên thư mục gốc của repository.
3. Vào **Settings → Pages**.
4. Trong phần Build and deployment, chọn **Deploy from a branch**.
5. Chọn branch `main`, folder `/ (root)`, rồi bấm **Save**.
6. Đợi GitHub Pages xuất bản website. Đường dẫn thường có dạng `https://TEN-TAI-KHOAN.github.io/TEN-REPOSITORY/`.

## Bước tiếp theo
Để cài bộ máy tính toán và luận giải đúng hệ thống riêng, hãy chuẩn bị:
1. Quy tắc tính từ ngày/tháng/năm/giờ sinh, gồm cách xử lý âm lịch/dương lịch.
2. Công thức lập Bảng Tâm Số và quy tắc điền đủ 12 cung.
3. Danh sách sao, yếu tố bổ sung và ý nghĩa theo từng cung.
4. Các mẫu luận giải chuẩn do Viên Minh Các cung cấp.
5. Ví dụ lá số đầu vào và kết quả đúng đã được xác nhận để kiểm thử.

## Riêng tư dữ liệu
Phiên bản này lưu dữ liệu trong trình duyệt trên thiết bị đang sử dụng; dữ liệu không tự đồng bộ sang thiết bị khác. Không dùng bản mẫu này để lưu hồ sơ nhạy cảm trên máy dùng chung.
