---
name: google-drive-report
description: Đọc dữ liệu chiến dịch từ Google Drive và tạo báo cáo hiệu suất quảng cáo
---

# google-drive-report

Kết nối Google Drive để đọc dữ liệu chiến dịch quảng cáo và tạo báo cáo hiệu suất tự động.

## Cách dùng

Cung cấp tên file hoặc link Google Sheet chứa dữ liệu chiến dịch. Skill sẽ:
1. Tìm và đọc dữ liệu từ Google Drive qua MCP
2. Phân tích các chỉ số: Chi tiêu, CTR, CPC, Lượt hiển thị, Chuyển đổi
3. Xuất báo cáo tóm tắt theo format chuẩn

## Đầu vào
```
File Google Sheet: [tên file hoặc link]
Kỳ báo cáo: [VD: Tháng 6/2026]
Kênh cần lọc: [Facebook / Google / TikTok / Tất cả]
```

## Đầu ra — Báo cáo hiệu suất

### Tóm tắt tổng quan
| Chỉ số | Giá trị | So sánh kỳ trước |
|--------|---------|-----------------|
| Tổng chi tiêu | | |
| Tổng lượt hiển thị | | |
| Tổng click | | |
| CTR trung bình | | |
| CPC trung bình | | |

### Phân tích theo kênh
Bảng so sánh hiệu suất Facebook / Google / TikTok.

### Top nhóm quảng cáo
- Top 3 nhóm chi tiêu cao nhất
- Top 3 nhóm CTR cao nhất
- Nhóm chưa đạt KPI (tiến độ < 60%)

### Khuyến nghị tối ưu
Dựa trên dữ liệu thực tế, đề xuất 3–5 action cụ thể.

---

## Kết nối MCP
Skill sử dụng Google Drive MCP: `search_files`, `read_file_content`, `get_file_metadata`, `create_file`.
