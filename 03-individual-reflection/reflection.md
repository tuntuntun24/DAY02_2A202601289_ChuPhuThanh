# Nhật Ký Phản Tư — Day 02 (Reflection Log)

## 1. Bài học tâm đắc nhất
- **Chuyển dịch từ "Solution-First" sang "Problem-First":** Trước đây, tôi thường có xu hướng nghĩ ngay đến việc tạo ra một "Chatbot AI toàn năng" có thể tự động trả lời mọi thứ. Tuy nhiên, sau bài lab này, tôi nhận ra giá trị lớn nhất nằm ở việc **mô hình hóa quy trình vận hành thủ công** và chỉ đưa AI vào đúng nút thắt (Bottleneck) để hỗ trợ phân loại và soạn nháp.
- **Sức mạnh của mô hình lai (Rule + Workflow + Human-in-the-loop):** Không cần phải xây dựng một Agent tự chủ phức tạp. Kết hợp giữa Rule tĩnh (cho câu hỏi đơn giản), AI (soạn nháp câu trả lời có trích dẫn) và Trợ giảng (phê duyệt cuối) là giải pháp tối ưu nhất về chi phí, tốc độ và độ an toàn.

## 2. Các bẫy (Anti-patterns) đã nhận diện và phòng tránh
- **Tránh bẫy "Mơ hồ hiện trạng" (No Baseline):** Đã lượng hóa được thiệt hại cụ thể (TA mất 3–4h/ngày, học viên chờ 45–60 phút) thay vì nói chung chung là "giúp tiết kiệm thời gian".
- **Tránh bẫy "Mập mờ ranh giới" (No Boundary):** Đặt ra giới hạn nghiêm ngặt: AI không được tự ý gửi câu trả lời kỹ thuật thẳng cho học viên và không được tự ý chấm điểm đạt/hỏng bài lab.
- **Tránh bẫy "Bỏ qua đường lui" (No Fallback):** Đã thiết kế phương án dự phòng khi AI bị timeout hoặc hallucination để không làm gián đoạn việc học của học viên.

## 3. Kế hoạch hành động tiếp theo
- Chuẩn bị bước sang **Day 07 & Day 08** để bắt tay vào kỹ thuật xây dựng hệ thống **RAG (Retrieval-Augmented Generation)**: nhúng toàn bộ slide, code mẫu và tài liệu bài giảng vào Vector Store để làm "bộ não tri thức" chuẩn xác cho AI tra cứu.
- Xây dựng bộ dữ liệu kiểm thử (Evaluation - Day 14) gồm 20 câu hỏi thực tế của học viên các khóa trước để đo lường độ chính xác của bản nháp trước khi đưa vào hỗ trợ thật.
