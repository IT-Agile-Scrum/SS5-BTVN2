# Phân biệt AC và Definition of Done thanh toán ví

| Phát biểu | Loại | Đạt/Chưa đạt | Lý do |
|---|---|---|---|
| Đ1 | AC | Đạt về cách viết | Mô tả số dư đủ và kết quả có thể kiểm tra. |
| Đ2 | DoD | Đạt | Quy định kiểm tra code có thể áp dụng chung cho mọi story. |
| Đ3 | AC | Chưa đạt | Đây là yêu cầu về tốc độ thanh toán nhưng “nhanh, mượt, thích” không đo được. |
| Đ4 | AC | Chưa đạt khi kiểm thử | Kết quả thực tế trừ tiền dù số dư không đủ, trái điều kiện thanh toán an toàn. |
| Đ5 | DoD | Chưa đạt về phạm vi | Chỉ nhắc story thanh toán, trong khi DoD phải dùng chung cho mọi story. |

## Sửa và kết luận

- Đ3: Given số dư đủ và hệ thống hoạt động bình thường, When khách xác nhận thanh toán, Then hệ thống hiển thị kết quả thanh toán trong vòng 3 giây. Ngưỡng 3 giây là đề xuất cần Product Owner xác nhận.
- Đ5: Mọi story đã triển khai trên staging và không còn lỗi Blocker hoặc Critical liên quan.

Story chưa hoàn thành vì trường hợp số dư không đủ vẫn bị trừ tiền. Developers sửa lỗi, kiểm thử lại toàn bộ AC và DoD trước khi báo hoàn thành.
