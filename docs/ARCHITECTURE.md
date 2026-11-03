# Kiến trúc hệ thống

## Các lớp
1. **Nguồn tri thức:** tài liệu Word/PDF, ghi chú bài giảng, khẩu quyết, bảng quy tắc và ca mẫu. Ghi mã nguồn, tác giả/nguồn, phiên bản, ngày nhận và quyền sử dụng.
2. **Chuẩn hóa tri thức:** chia tài liệu thành đơn vị có thể trích dẫn, giữ trang/đoạn, chủ đề, trạng thái xác minh.
3. **Rule Engine:** lưu quy tắc có phiên bản, điều kiện, đầu vào, kết quả, ngoại lệ, ví dụ và trạng thái duyệt. LLM không được tự thay đổi quy tắc.
4. **Calculation Engine:** thực hiện phép tính xác định. Chỉ triển khai khi công thức và quy ước được xác nhận; mỗi hàm có unit test.
5. **Retrieval / RAG:** tìm đoạn tài liệu liên quan và giữ metadata nguồn. Điểm tương đồng không đồng nghĩa với tính đúng.
6. **LLM Orchestrator:** gọi công cụ tính, truy xuất tri thức, sau đó diễn giải theo quy tắc; phải phân biệt dữ kiện, diễn giải và dự báo.
7. **Evaluation:** kiểm tra độ chính xác phép tính, tuân thủ quy tắc, trích dẫn, phát hiện dữ kiện thiếu và tỷ lệ khẳng định vô căn cứ.

## Luồng xử lý
1. Chuẩn hóa và xác thực đầu vào.
2. Kiểm tra dữ liệu bắt buộc, mâu thuẫn.
3. Gọi calculation engine cho phép tính xác định.
4. Truy xuất tri thức đúng hệ thống/chủ đề/phiên bản.
5. Tạo gói ngữ cảnh kèm nguồn.
6. LLM diễn giải, không tự thêm quy tắc chưa có.
7. Validator kiểm tra nguồn, mâu thuẫn và trường bắt buộc.
8. Trả báo cáo kèm căn cứ và mức bất định.

## Trạng thái tri thức
- `confirmed`: đã được người phụ trách duyệt.
- `proposed`: đề xuất, chưa duyệt.
- `reference`: tài liệu tham khảo, chưa phải quy tắc riêng.
- `deprecated`: đã thay thế, giữ lịch sử.
- `conflict`: đang có mâu thuẫn cần xử lý.

## Ranh giới
RAG không phải huấn luyện mô hình; RAG giúp tìm tài liệu lúc trả lời. Fine-tuning là giai đoạn riêng, chỉ cân nhắc sau khi dữ liệu sạch, có quyền sử dụng và có tập đánh giá độc lập.

## Bảo mật
Tài liệu có bản quyền và hồ sơ khách hàng nên lưu ở kho private. Secret lưu trong secret manager/environment variables. Xây dựng cơ chế phân quyền, xuất và xóa dữ liệu cá nhân.