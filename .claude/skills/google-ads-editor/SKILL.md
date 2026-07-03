---
name: google-ads-editor
description: Chuẩn hóa dữ liệu chiến dịch thành 2 bảng format Google Ads Editor để upload
---

# google-ads-editor

Sắp xếp dữ liệu chiến dịch thành đúng 2 bảng format Google Ads Editor để paste vào Google Sheet và upload.

## Dữ liệu đầu vào cần cung cấp

### 1. Cấu trúc chiến dịch & từ khóa
```
Campaign: [tên campaign]
Ad Group: [tên ad group] → từ khóa: [kw1], [kw2], [kw3]
Ad Group: [tên ad group] → từ khóa: [kw1], [kw2]
```

### 2. Nội dung quảng cáo (theo từng Ad Group)
```
Ad Group: [tên]
Headline: [H1] / [H2] / [H3] / ...
Description: [D1] / [D2]
```

### 3. Path & URL
```
Ad Group [tên]: path1 = [x], path2 = [y], url = [https://...]
```

---

## Yêu cầu đầu ra

### Bảng 1 — Keyword List
Cột: `Campaign | Ad group | Keyword | Criterion Type`

- Criterion Type = phrase cho tất cả
- Mỗi từ khóa 1 dòng, giữ nguyên dấu/không dấu như dữ liệu gốc
- Mỗi chủ đề từ khóa chỉ gộp vào 1 Ad Group duy nhất

### Bảng 2 — RSA Ads
Cột: `Campaign | Ad Group | Headline 1 | [ký tự] | Headline 2 | [ký tự] | ... Headline 15 | [ký tự] | Description 1 | [ký tự] | Description 2 | [ký tự] | Description 3 | [ký tự] | Description 4 | [ký tự] | Path 1 | 15 | Path 2 | 15 | Final URL`

- Không viết lại, không thêm bớt nội dung — chỉ chuẩn hóa format
- Sau mỗi headline/description ghi đúng số ký tự thực tế (kể cả dấu cách)
- Nếu thiếu headline/description thì để trống ô đó
- Mỗi Ad Group = 1 dòng trong bảng
- Giữ nguyên cấu trúc cột để paste thẳng vào Google Sheet
