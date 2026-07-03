---
name: keyword-ggads
description: Research từ khóa Google Ads bằng KeywordTool.io, xuất bảng kèm Search Volume
---

# keyword-ggads

Sử dụng KeywordTool.io để lên bộ từ khóa Google Ads cho các nhóm sản phẩm/dịch vụ, kèm Search Volume.

## Mục tiêu
- Tạo bộ từ khóa phù hợp để chạy Google Search Ads
- Ưu tiên từ khóa có nhu cầu tìm kiếm thực tế, đúng intent mua
- Kết quả dễ copy sang Google Sheet theo đúng bảng mẫu

## Quy tắc dùng KeywordTool
- Chỉ check quota 1 lần ở đầu
- Không gọi suggestions lan man, không mở rộng quá xa nhóm sản phẩm chính
- Chỉ gọi search-volume theo danh sách từ khóa phù hợp
- Không check quota nhiều lần trong quá trình làm
- Tối ưu quota: ưu tiên lấy Search Volume chính xác cho từ khóa có khả năng dùng chạy Ads
- Không chia volume theo tỉnh — chỉ lấy tổng theo tất cả khu vực đã chọn
- Loại bỏ từ khóa không liên quan, quá chung chung hoặc sai intent
- Không trùng lặp từ khóa giữa các nhóm nếu intent đã quá giống nhau

## Yêu cầu sắp xếp
- Trong từng nhóm: sắp xếp keyword theo Search Volume từ cao xuống thấp
- Chỉ giữ keyword có volume phù hợp để dùng cho Google Ads

## Yêu cầu xuất bảng
- Xuất thành 1 bảng duy nhất, format giống mẫu Google Sheet
- Mỗi nhóm từ khóa là 1 cụm cột riêng đặt cạnh nhau
- Mỗi cụm gồm 2 cột: `Keywords | Search volume`
- Header nhóm viết in hoa, nền xanh đậm, chữ trắng
- Search volume định dạng số có dấu chấm phân tách hàng nghìn (VD: 1.500)
- Bảng cần dễ copy trực tiếp sang Google Sheet

## Cấu trúc bảng mong muốn
```
[NHÓM SẢN PHẨM A]          [NHÓM SẢN PHẨM B]
Keywords | Search volume    Keywords | Search volume
```
