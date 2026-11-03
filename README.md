# Viên Minh Các — AI huyền học và kho tri thức

Dự án phát triển trợ lý AI chuyên môn cho hệ thống kiến thức của Viên Minh Các. Giai đoạn đầu ưu tiên **Bát Tự Manh Phái** và **Tâm Số Học**, đồng thời chuẩn bị cấu trúc để mở rộng.

## Mục tiêu
1. Lưu trữ tài liệu nguồn có nguồn gốc và phiên bản.
2. Chuẩn hóa quy tắc riêng thành dữ liệu có cấu trúc, phân biệt với kiến thức tham khảo.
3. Dùng bộ máy tính toán xác định cho phép tính có thể kiểm thử.
4. Dùng RAG để truy xuất tài liệu nền và giữ nguồn trích dẫn nội bộ.
5. Tạo báo cáo phân biệt dữ kiện, diễn giải, giả thuyết và dự báo.
6. Kiểm thử bằng ca mẫu đã được người phụ trách chuyên môn xác nhận.

## Trạng thái hiện tại
Repository đã có website tĩnh lập lá số Tâm Số Học tại `index.html`. Giữ nguyên website đó. Nhánh này chỉ bổ sung nền móng tài liệu và cấu trúc dữ liệu; chưa phải AI đã huấn luyện, chưa có API mô hình và chưa tự tính Bát Tự hay sinh luận giải tự động.

## Cấu trúc
- `knowledge_base/`: tài liệu và tri thức chuẩn hóa.
- `rules/`: quy tắc nghiệp vụ do Viên Minh Các quản lý.
- `schemas/`: định dạng dữ liệu.
- `calculation_engine/`: thuật toán tính toán xác định.
- `ai_engine/`: truy xuất tri thức và điều phối mô hình.
- `evaluation/`: bộ ca kiểm thử và tiêu chí đánh giá.
- `docs/`: kiến trúc, quy trình nhập liệu và quản trị.
- `data/examples/`: dữ liệu minh họa không chứa thông tin cá nhân thật.

## Nguyên tắc quản trị
- Không tự suy diễn rồi ghi thành quy tắc chính thức.
- Mỗi quy tắc có mã, nguồn, phiên bản, người duyệt và trạng thái.
- Phân biệt `source_fact`, `system_rule`, `derived_interpretation`, `prediction` và `case_observation`.
- Quy tắc mới ở trạng thái `proposed` cho đến khi người phụ trách phê duyệt.
- Khi có mâu thuẫn, lưu lại hai quan điểm và tạo mục cần xác minh.
- Không commit dữ liệu lá số có thể nhận diện cá nhân vào repository công khai.

## Quy trình phát triển
1. Tiếp nhận tài liệu và ghi nguồn/quyền sử dụng.
2. Trích xuất, phân loại và chuẩn hóa.
3. Tạo bản ghi quy tắc theo schema.
4. Người phụ trách chuyên môn duyệt.
5. Viết thuật toán khi công thức đã được xác nhận.
6. Tạo ca kiểm thử gồm đầu vào, kết quả kỳ vọng và căn cứ.
7. Chỉ bật quy tắc trong phiên bản vận hành khi đạt kiểm thử.

## Riêng tư và bảo mật
Không commit API key, mật khẩu, token hoặc hồ sơ khách hàng. Dùng biến môi trường và kho lưu trữ riêng cho dữ liệu nhạy cảm. Kiểm tra quyền sử dụng tài liệu trước khi đưa vào dịch vụ bên thứ ba.
