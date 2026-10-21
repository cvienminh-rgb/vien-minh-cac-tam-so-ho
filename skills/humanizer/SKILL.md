---
name: humanizer
description: Gỡ các dấu hiệu khiến bài đọc lên như AI viết (nhịp câu đều, mở kết rập khuôn, giọng trung tính, liệt kê máy móc) mà giữ nguyên nội dung. Dùng khi người dùng muốn bài tự nhiên như người thật viết, hoặc gõ /humanizer.
---

# Gỡ sạch dấu hiệu văn AI

Kiểm tra và sửa lần lượt:
1. **Nhịp câu:** AI hay viết các câu dài bằng nhau. Xen câu ngắn với câu dài, cho phép câu chỉ 3 đến 4 chữ.
2. **Mở bài:** bỏ câu dẫn chung chung ("Ngày nay..."). Vào thẳng ý chính hoặc chi tiết cụ thể nhất.
3. **Kết bài:** bỏ đoạn tóm tắt lại những gì vừa nói, bỏ câu kêu gọi kiểu khẩu hiệu.
4. **Liệt kê:** nếu bài toàn gạch đầu dòng, chuyển phần nên kể thành câu văn.
5. **Giọng:** làm rõ chính kiến và chi tiết cụ thể đã có, bỏ câu rào đón ("có thể nói", "phần nào").
6. **Dấu câu:** bớt dấu gạch ngang dài, dấu hai chấm và in đậm.
7. **Emoji:** tối đa 1 đến 2 cái nếu giọng bài cho phép, không đặt ở đầu mỗi dòng.

Giữ nguyên ý, số liệu, tên riêng. Không thêm thông tin mới.
Trả về bài đã sửa, không giải thích trừ khi người dùng hỏi.
