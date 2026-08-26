# Individual Problem Scan — Day 02

> Ghi chú: Bài tập cá nhân tập trung đào sâu một bài toán thực tế có thật thay vì scan dàn trải. Các số liệu baseline được lượng hóa dựa trên quy mô lớp học 1.000 học viên.

## Problem đã chọn

| Trường | Nội dung |
|---|---|
| **Lăng kính** | Lặp lại + Tốn thời gian + Điểm đau người dùng |
| **Problem** | Trợ giảng (TA/Lab Coach) bị quá tải vì phải rà soát thủ công các câu hỏi trùng lặp và yêu cầu hỗ trợ thiếu thông tin, khiến thời gian phản hồi bị kéo dài và học viên bị tắc nghẽn khi làm lab. |
| **Actor** | Trợ giảng (Lab Coach/TA) và Học viên trong lớp học quy mô lớn (1.000 học viên). |
| **Tần suất** | Xảy ra liên tục trong các buổi thực hành Lab và suốt tuần làm bài tập. |
| **Dấu hiệu thật** | Kênh hỗ trợ ngập tràn các câu hỏi cơ bản lặp đi lặp lại hoặc các câu hỏi chỉ gửi ảnh chụp lỗi mờ, thiếu mô tả chi tiết và ngữ cảnh. |

---

## Problem Card

- **Problem 1 câu:** Trợ giảng bị quá tải vì phải rà soát thủ công các câu hỏi trùng lặp và các yêu cầu hỗ trợ thiếu thông tin, khiến thời gian phản hồi kéo dài và học viên bị tắc nghẽn khi thực hành.
- **Thời điểm / bối cảnh:** Trong các buổi thực hành lab trực tuyến và cao điểm nộp bài tập hàng tuần.
- **Current workflow:**
  1. Học viên gặp lỗi hoặc tắc nghẽn khi làm bài lab.
  2. Học viên gửi câu hỏi lên kênh Discord / Form hỗ trợ.
  3. Trợ giảng mở từng tin nhắn, đọc ngữ cảnh, phát hiện câu hỏi thiếu mã lỗi hoặc ảnh chụp không rõ ràng.
  4. Trợ giảng nhắn tin hỏi lại hoặc copy-paste câu trả lời từ tài liệu bài giảng cũ.
  5. Học viên nhận phản hồi, bổ sung thông tin và chỉnh sửa bài làm.
- **Bottleneck:** Khâu Trợ giảng phải đọc từng tin nhắn để phân loại thủ công và đi đòi thêm thông tin ngữ cảnh.
- **Impact (Baseline):** 
  - Trợ giảng mất 3–4 tiếng/ngày cho các tác vụ hỗ trợ lặp lại.
  - Học viên phải chờ trung bình 45–60 phút để nhận được phản hồi đầu tiên.
- **Success metric dự kiến:** 
  - Rút ngắn thời gian phản hồi trung bình cho học viên xuống dưới 5 phút.
  - Cắt giảm 50% thời gian xử lý các câu hỏi trùng lặp của Trợ giảng.
  - Không làm tăng tỷ lệ khiếu nại hoặc hướng dẫn sai lệch.
- **Non-AI alternative:** Tạo trang FAQ tĩnh + thiết lập Form yêu cầu bắt buộc đính kèm log lỗi. *(Hạn chế: Học viên ngại đọc tài liệu dài, Form tĩnh không hiểu được ngữ cảnh đa dạng của câu hỏi)*.
- **AI hypothesis:** AI đóng vai trò phân loại (Triage) câu hỏi, tự động nhắc học viên bổ sung thông tin nếu thiếu, và tra cứu tài liệu bài giảng để soạn sẵn bản nháp câu trả lời có trích dẫn nguồn cho Trợ giảng duyệt.
- **Quick gut:** Cấp độ **Workflow** kết hợp **Rule**.

---

## Draft workflow hiện tại

```text
[Học viên gặp lỗi khi làm lab]
        ↓
[Gửi câu hỏi lên kênh hỗ trợ]
        ↓
[Trợ giảng đọc ngữ cảnh, phát hiện thiếu thông tin]  <-- BOTTLENECK
        ↓
[Trợ giảng hỏi lại hoặc copy câu trả lời cũ]
        ↓
[Học viên bổ sung thông tin & sửa bài]
