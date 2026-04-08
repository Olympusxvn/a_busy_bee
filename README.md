# 🐝 A Busy Bee

> *Chỉ 3 công cụ. Không phức tạp. Tiết kiệm token.*

| Công cụ | Dùng để | Token |
|---------|---------|-------|
| **GSD** | Lập kế hoạch, checklist, tài liệu | ~200-400 |
| **Everything** | Code, review, bảo mật (qua subagent) | ~800-2000 |
| **Superpowers** | Debug khó, TDD | ~1200-1500 |

## Cách dùng
1. Clone repo này
2. Mở Claude Code
3. Nói: *"Ong Con ơi, hãy lập kế hoạch cho module X"*

## Quy trình mẫu
- GSD: lập kế hoạch → lưu file
- Everything (subagent): code theo spec
- Everything (review): kiểm tra code
- Superpowers (nếu lỗi): debug
