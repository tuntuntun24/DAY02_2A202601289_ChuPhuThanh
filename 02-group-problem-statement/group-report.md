# Team Problem Statement & Decision Gate — Day 02

## 1. Problem Statement Hoàn Chỉnh (9 Trường Thông Tin)

### A. 6 Yếu Tố Bài Toán Cốt Lõi (Core Problem)

1. **Actor (Đối tượng chịu ảnh hưởng):**
   - Trợ giảng (Lab Coach/TA) trực tiếp quản lý và hỗ trợ giải đáp thắc mắc cho lớp học quy mô lớn (1.000 học viên).

2. **Workflow (Quy trình vận hành hiện tại):**
   - Bước 1: Học viên gặp lỗi/tắc nghẽn khi làm lab và gửi câu hỏi lên kênh hỗ trợ.
   - Bước 2: Trợ giảng mở từng câu hỏi, đọc ngữ cảnh và mã lỗi.
   - Bước 3: Trợ giảng nhắn tin yêu cầu bổ sung thông tin (nếu câu hỏi mơ hồ, thiếu log, ảnh mờ).
   - Bước 4: Trợ giảng tra cứu tài liệu bài giảng cũ và gõ/copy câu trả lời gửi cho học viên.
   - Bước 5: Học viên nhận phản hồi, chỉnh sửa code và tiếp tục làm bài.

3. **Bottleneck (Nút thắt cổ chai):**
   - Khâu đọc, phân loại thủ công và đi đòi thêm thông tin ngữ cảnh cho các câu hỏi thiếu dữ liệu chiếm phần lớn thời gian của Trợ giảng.

4. **Impact (Tổn thất định lượng / Baseline):**
   - Trợ giảng mất **3–4 giờ/ngày** cho các tác vụ hỗ trợ lặp lại.
   - Học viên phải chờ trung bình **45–60 phút** để nhận được phản hồi, gây đứt mạch học tập và tăng tỷ lệ bỏ ngang bài lab.

5. **Success Metric (Chỉ số thành công đo được):**
   - Rút ngắn thời gian phản hồi trung bình cho học viên xuống **dưới 5 phút**.
   - Giảm **50% thời gian** xử lý câu hỏi lặp của Trợ giảng.
   - **Quy tắc hành động (PAIR Rule):** *Nếu tỷ lệ bản nháp AI bị Trợ giảng sửa > 30% trong 2 tuần liên tiếp, hệ thống sẽ tự động hạ mức tự động hóa về Pha 1 (chỉ gợi ý tài liệu, không soạn sẵn câu trả lời).*

6. **Boundary (Ranh giới kiểm soát):**
   - AI **KHÔNG** được tự ý gửi câu trả lời kỹ thuật chuyên sâu thẳng cho học viên mà chưa có sự phê duyệt của Trợ giảng.
   - AI **KHÔNG** được tự ý chấm điểm hay đưa ra phán quyết Đạt/Không đạt bài lab của học viên.

---

### B. 3 Yếu Tố Quyết Định Công Nghệ AI (AI Technical Decisions)

7. **Điểm can thiệp (Decision Entry):**
   - Can thiệp ngay tại khâu tiếp nhận câu hỏi của học viên: tự động kiểm tra độ đầy đủ của ngữ cảnh và tự động soạn sẵn bản nháp câu trả lời kèm nguồn trích dẫn từ bài giảng.

8. **Mức chọn giải pháp (Decision Level):**
   - **Workflow kết hợp Rule tĩnh** (Cấp độ 2): Dùng Rule để tự gửi link/tài liệu cho các câu hỏi cơ bản cố định; dùng AI Workflow để phân tích ngữ cảnh, nhắc bổ sung thông tin và soạn nháp câu trả lời.

9. **Rủi ro & Human-in-the-loop (Decision Safety):**
   - **Rủi ro chính:** AI có thể bị ảo giác (hallucination), trích dẫn sai bài giảng hoặc đưa ra hướng dẫn lỗi thời khiến học viên làm sai bài lab.
   - **Cơ chế HITL:** Toàn bộ câu trả lời kỹ thuật đều được đưa vào hàng đợi kiểm duyệt (Review Queue); Trợ giảng đọc lướt, chỉnh sửa nếu cần và bấm "Phê duyệt (Approve)" thì câu trả lời mới được gửi đi.

---

## 2. Thẩm Định Qua 5 Câu Hỏi Gate Quyết Định

| STT | Câu hỏi kiểm tra mức sẵn sàng | Đánh giá | Lập luận chi tiết |
|:---:|---|:---:|---|
| **01** | Nghiệp vụ có đòi hỏi xử lý ngôn ngữ, tri thức chuyên môn hoặc suy luận? | **Có** | Học viên hỏi bằng tiếng Việt tự nhiên với muôn vàn cách diễn đạt khác nhau; cần hiểu ngữ cảnh lỗi lập trình và tra cứu đúng kiến thức bài giảng. |
| **02** | Dữ liệu đầu vào có cung cấp đủ ngữ cảnh để AI phản hồi chính xác? | **Có** | Hệ thống có sẵn toàn bộ slide bài giảng, code lab mẫu, và tài liệu lý thuyết chuẩn mực của khóa học làm dữ liệu đối chứng (Ground Truth). |
| **03** | Đã thiết lập các chỉ số định lượng để đánh giá hiệu quả? | **Có** | Đã xác định rõ Baseline (45-60 phút chờ) và Target (< 5 phút), kèm theo quy tắc hành động điều chỉnh mức tự động hóa khi tỷ lệ sửa > 30%. |
| **04** | Hậu quả khi AI sai sót có nằm trong phạm vi kiểm soát? | **Có** | Kiểm soát an toàn 100% nhờ chốt chặn Trợ giảng (Human-in-the-loop) duyệt toàn bộ bản nháp trước khi gửi tới học viên. |
| **05** | Có giải pháp thay thế đơn giản và tối ưu chi phí hơn AI không? | **Không** | Các giải pháp phi-AI như FAQ hay biểu mẫu tĩnh đã bộc lộ rõ hạn chế do học viên ngại đọc văn bản dài và câu hỏi thực tế có độ biến thiên ngữ nghĩa rất cao. |

---

## 3. Khung Ra Quyết Định Cuối Cùng

### 🚦 Quyết định: **`Go` (Đủ điều kiện triển khai)**

**Lập luận bảo vệ:** 
- Bài toán có điểm đau rõ ràng, tần suất lặp lại cao với quy mô 1.000 học viên.
- Ranh giới giữa Trợ giảng và AI được phân định mạch lạc, đảm bảo trải nghiệm học tập luôn được kiểm soát chất lượng tuyệt đối.
- Bước tiếp theo là triển khai xây dựng bộ nhớ vector (Day 07) và luồng RAG (Day 08) để kết nối tri thức bài giảng cho hệ thống.
