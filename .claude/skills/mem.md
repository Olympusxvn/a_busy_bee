# Mem - Bộ nhớ đơn giản cho Ong Con
# Lưu bài học, quyết định, context giữa các session vào file markdown.
# Không DB, không worker, không tốn token cho AI compression.

## Cách dùng

### /mem save <nội dung>
Lưu 1 ghi chú vào `docs/mem/`. Tên file = ngày + slug tự động.
Ví dụ: `docs/mem/2026-04-22_auth-module-decision.md`

Format ghi chú:
```
---
date: YYYY-MM-DD
tags: [tag1, tag2]
---
Nội dung ghi chú
```

### /mem list
Liệt kê ghi chú gần đây (10 gần nhất).

### /mem search <từ khóa>
Tìm trong tất cả ghi chú bằng grep.

## Quy tắc
- Mỗi ghi chú là 1 file markdown riêng trong `docs/mem/`
- Tên file: `YYYY-MM-DD_slug.md` (slug = 3-5 từ viết-thường, nối bằng dấu gạch)
- Tags giúp phân loại: `decision`, `lesson`, `bug`, `plan`, `context`
- Cuối session, nhắc user: "Có gì cần /mem save không?"
- Không lưu code, chỉ lưu bài học / quyết định / context
- Giữ mỗi ghi chú ngắn gọn, dưới 20 dòng
