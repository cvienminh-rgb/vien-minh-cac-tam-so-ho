---
name: auto-block-banned-words
description: Tự động chặn các từ và cụm từ mà thương hiệu hoặc người dùng cấm, theo danh sách trong references/tu-cam.txt, trước khi trả bài. Dùng mỗi khi viết hoặc sửa nội dung để đăng, khi người dùng nhắc đến từ cấm, hoặc gõ /auto-block-banned-words.
---

# Tự động chặn từ bị cấm

1. Đọc danh sách trong `references/tu-cam.txt`. Mỗi dòng là một từ hoặc cụm từ bị cấm; dòng bắt đầu bằng # là ghi chú.
2. Trước khi trả bất kỳ bài nào, rà toàn bộ bài, không phân biệt hoa thường, tính cả cách viết không dấu.
3. Gặp từ cấm: viết lại câu để giữ ý mà không dùng từ đó. Nếu không giữ được ý (ví dụ một lời cam kết không có căn cứ), xoá câu và báo người dùng.
4. Cuối câu trả lời ghi "Đã chặn: ..." kèm danh sách, hoặc "Không có từ cấm".
5. Người dùng muốn thêm từ: hướng dẫn họ thêm một dòng vào `references/tu-cam.txt`.

Nếu không đọc được file, dùng danh sách mặc định: giá rẻ nhất, cam kết 100%, số 1 Việt Nam, tốt nhất thị trường, tuyệt đối, chữa khỏi, hiệu quả ngay lập tức, không tác dụng phụ.
