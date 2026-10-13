# BÁO CÁO RÀ SOÁT VÀ HIỆU CHỈNH SỐ LIỆU SPRINT 4 - DỰ ÁN RIKKEIGO

> 👤 **Học viên:** Đỗ Hoàng Sơn | **Mã SV:** PTIT-HCM-066
> 🏫 **Môn học:** IT206-K25-Agile-va-Scrum

---

## Phần 1 - Phân tích: Đánh giá các nhận định báo cáo của Tú

Sau khi rà soát báo cáo của Tú dựa trên các quy tắc nghiệp vụ của Scrum và dữ liệu thực tế của Sprint 4, tôi nhận thấy có nhiều điểm chưa chính xác về mặt logic và nguyên tắc tính toán. Việc 'làm đẹp' số liệu hoặc hiểu sai về cách vận hành Burndown Chart sẽ gây ảnh hưởng nghiêm trọng đến tính minh bạch (Transparency) và khả năng lập kế hoạch cho các Sprint tiếp theo.

| Nhận định | Đúng / Sai | Căn cứ trong dữ liệu | Hậu quả nếu giữ nguyên |
| --- | --- | --- | --- |
| BC1. Velocity Sprint 4 = 21 SP | Sai | Velocity chỉ tính tổng SP của các PBI đạt DoD (Done). PBI RikkeiPay (8 SP) chưa xong Integration Test nên tính là 0 SP. | Gây ảo tưởng về năng suất thực tế của đội, dẫn đến việc 'ép' khối lượng công việc quá tải ở Sprint sau. |
| BC2. Ngày 1-2 đi ngang cần kiểm tra Task | Đúng | Đường Actual Line nằm ngang nghĩa là không có SP nào được hoàn thành (giải phóng) trong giai đoạn này. | Giúp đội phát hiện sớm các điểm nghẽn (bottleneck) hoặc tình trạng làm dở dang quá nhiều việc (WIP) cùng lúc. |
| BC3. Ngày 3 đường tăng do làm chậm | Sai | Ngày 3 đường tăng từ 21 lên 24 do thêm PBI 'Hiển thị mã khuyến mãi' (3 SP) vào Sprint Backlog (Scope Creep). | Đổ lỗi sai cho Developers, che lấp vấn đề quản lý phạm vi (Scope) không ổn định trong Sprint. |
| BC4. Ngày 10 sửa số về 0 cho đẹp | Sai | PBI RikkeiPay chưa Done nên thực tế vẫn còn 8 SP chưa hoàn thành. Số liệu đúng phải là 8 thay vì 0. | Vi phạm tính minh bạch của Scrum. Quản lý sẽ không biết dự án đang bị chậm tiến độ thực tế. |
| BC5. PBI RikkeiPay tự chuyển sang Sprint 5 với 2 SP | Sai | PBI chưa Done phải quay về Product Backlog để PO xem xét lại. Không được tự ý chia nhỏ SP khi tính Velocity. | Phá vỡ quy trình lập kế hoạch Sprint (Sprint Planning) và làm sai lệch cách tính Velocity của các Sprint. |

## Phần 2 - Vá lỗi: Hiệu chỉnh số liệu và Phương án xử lý

Dựa trên các phân tích ở Phần 1, tôi thực hiện tính toán lại các chỉ số quan trọng để đảm bảo báo cáo phản ánh đúng thực tế năng lực của đội ngũ.

- Tính lại Velocity Sprint 4: Chỉ cộng các PBI đã Done (Hủy chuyến: 5 + Đánh giá: 5 + Địa chỉ: 3 + Ảnh đại diện: 2). Phép tính: 5 + 5 + 3 + 2 = 15 SP.
- Số SP còn lại đúng của ngày 10: 8 SP (Đây chính là số điểm của PBI 'Thanh toán bằng ví RikkeiPay' chưa đạt DoD).
- Cách xử lý PBI ví RikkeiPay: PBI này phải được chuyển trả về Product Backlog. Product Owner (PO) sẽ đánh giá lại độ ưu tiên của nó so với các yêu cầu mới. Nếu PO quyết định đưa vào Sprint 5, đội Developers sẽ ước lượng lại phần công việc còn lại để đưa vào Sprint Backlog, nhưng tuyệt đối không được tính 6 SP đã làm vào Velocity của Sprint 4.

---

## 📁 Danh sách tệp tin nộp bài trong Repository
- 📝 `bt2.docx`: Báo cáo tài liệu phân tích nghiệp vụ hoàn chỉnh.
