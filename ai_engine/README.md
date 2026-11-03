# AI Engine

Định hướng thành phần:
1. Retriever lấy các đoạn tri thức liên quan.
2. Rule resolver chọn quy tắc confirmed theo phiên bản.
3. Calculation adapter gọi hàm tính toán.
4. Prompt/orchestrator yêu cầu LLM diễn giải dựa trên dữ liệu và nguồn.
5. Output validator rà soát nguồn, mâu thuẫn, trường bắt buộc và tuyên bố thiếu căn cứ.

Không lưu API key trong mã nguồn. Chưa chọn nhà cung cấp LLM cho đến khi thống nhất mô hình, chính sách dữ liệu và ngân sách.