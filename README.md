# Claude Code Workspace — SEONGON Ads

Không gian làm việc cá nhân sử dụng [Claude Code Skills](https://docs.claude.com/claude-code) để hỗ trợ công việc chạy quảng cáo (Google Ads / Facebook Ads) tại SEONGON: viết nội dung quảng cáo, research từ khóa, chuẩn hóa dữ liệu upload, và đọc báo cáo hiệu suất từ Google Drive.

## Cấu trúc

```
.claude/skills/
├── ad-coppy/               # Viết & chuẩn hóa nội dung RSA (Google Ads)
│   └── SKILL.md
├── google-ads-editor/       # Chuẩn hóa dữ liệu thành 2 bảng format Google Ads Editor
│   └── SKILL.md
├── google-drive-report/     # Đọc dữ liệu từ Google Drive, tạo báo cáo hiệu suất
│   └── SKILL.md
└── keyword-ggads/           # Research từ khóa bằng KeywordTool.io, kèm Search Volume
    ├── SKILL.md
    ├── huong-dan.md          # Hướng dẫn quy tắc dùng KeywordTool chi tiết
    └── sample-output.md      # Mẫu bảng output tham khảo

outputs/                     # File output thực tế khi chạy các skill ở trên
```

## Danh sách skills

| Skill | Chức năng | Kết nối ngoài | File kèm theo |
|---|---|---|---|
| `ad-coppy` | Viết/chuẩn hóa nội dung RSA tiếng Việt cho Google Ads | – | – |
| `google-ads-editor` | Sắp xếp dữ liệu chiến dịch thành bảng Keyword List + RSA Ads đúng format Google Ads Editor | – | – |
| `google-drive-report` | Tìm & đọc dữ liệu chiến dịch trên Google Sheet, phân tích chỉ số, xuất báo cáo hiệu suất | ✅ Google Drive qua **MCP** (`search_files`, `read_file_content`, `get_file_metadata`, `create_file`) | – |
| `keyword-ggads` | Research bộ từ khóa Google Ads kèm Search Volume | ✅ **KeywordTool.io** (API) | ✅ `huong-dan.md`, `sample-output.md` |

Điều kiện bài tập:
- ≥ 3 skills trong `.claude/skills/` ✓ (4 skills)
- ≥ 1 skill kết nối nền tảng ngoài (API/MCP/CLI) ✓ (`google-drive-report` dùng MCP, `keyword-ggads` dùng API KeywordTool.io)
- ≥ 1 skill có file/folder kèm `SKILL.md` ✓ (`keyword-ggads`)

## Cách dùng

Trong Claude Code, tại thư mục repo này, gõ `/ad-coppy`, `/google-ads-editor`, `/google-drive-report` hoặc `/keyword-ggads` kèm mô tả sản phẩm/dữ liệu cần xử lý.

## Output mẫu

Xem thư mục [`outputs/`](./outputs) — kết quả thực tế khi chạy `ad-coppy` và `google-ads-editor` cho sản phẩm "sim số đẹp".
