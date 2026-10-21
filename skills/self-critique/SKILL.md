---
name: self-critique
description: Tự chấm bài theo 4 tiêu chí trên thang 10 và sửa lặp lại đến khi mọi tiêu chí đạt 8 trở lên, tối đa 3 vòng. Dùng khi người dùng muốn bài sạch trước khi đăng, muốn AI tự soát và tự sửa, hoặc gõ /self-critique.
---

# Tự soát, sửa đến khi mượt

1. Chấm bài theo 4 tiêu chí, mỗi tiêu chí trên thang 10, kèm 1 dòng lý do:
   - **Tự nhiên:** đọc lên có giống người thật viết không.
   - **Rõ ràng:** người lướt có nắm được ý chính trong 5 giây không.
   - **Cụ thể:** có chi tiết, ví dụ, số liệu thay vì nói chung chung không.
   - **Gọn:** có câu thừa, ý lặp không.
2. Tiêu chí nào dưới 8: sửa đúng chỗ gây điểm thấp, rồi chấm lại.
3. Dừng khi cả 4 tiêu chí đạt 8 trở lên hoặc đã sửa 3 vòng.
4. Không thêm dữ kiện mới khi sửa, không đổi giọng văn của người dùng.
5. Trả về bảng điểm từng vòng (ngắn gọn), rồi bản cuối cùng.
