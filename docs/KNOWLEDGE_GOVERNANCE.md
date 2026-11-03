# Quy chuẩn quản trị kho tri thức

## Phân loại nội dung
| Loại | Ý nghĩa | Dùng như quy tắc chính thức? |
|---|---|---|
| source_fact | Nội dung đọc được từ nguồn | Không tự động |
| system_rule | Quy tắc do Viên Minh Các xác lập | Chỉ khi confirmed |
| derived_interpretation | Diễn giải từ dữ kiện và quy tắc | Phải nêu căn cứ |
| prediction | Nhận định về khả năng tương lai | Phải nêu bất định |
| case_observation | Quan sát từ một ca | Không tự khái quát khi chưa duyệt |

## Trạng thái
`proposed` → `under_review` → `confirmed` → `deprecated`. Dùng `conflict` khi có nội dung mâu thuẫn. Không xóa lịch sử; tạo phiên bản mới và liên kết `supersedes`.

## Tiếp nhận tài liệu
1. Gán source_id.
2. Ghi tiêu đề, tác giả/đơn vị, phiên bản, ngày nhận và quyền sử dụng.
3. Giữ nguyên bản gốc.
4. Trích xuất theo trang/đoạn.
5. Gắn hệ thống và chủ đề.
6. Đánh dấu đoạn chưa rõ hoặc lỗi trích xuất để kiểm tra.
7. Tạo rule_id khi đề xuất quy tắc và ghi rõ nguồn.
8. Chờ người phụ trách duyệt trước khi đặt trạng thái confirmed.

## Xử lý mâu thuẫn
Lưu các rule/source liên quan, nội dung khác biệt, phạm vi áp dụng, câu hỏi cần quyết định và kết luận cuối cùng. Không tự động hợp nhất hai quy tắc xung đột.

## Nguyên tắc AI
- Ưu tiên quy tắc confirmed thuộc đúng phiên bản hệ thống.
- Không biến reference/proposed thành khẳng định.
- Không tự tạo công thức khi thiếu dữ kiện.
- Khi thiếu căn cứ, nêu rõ dữ kiện còn thiếu.
- Trích nguồn nội bộ bằng source_id, trang/đoạn và rule_id.
- Dự báo phải được gọi tên là dự báo, không viết như sự kiện chắc chắn.