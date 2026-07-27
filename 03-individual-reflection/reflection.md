# 03 — Individual Reflection

**Học viên:** Chu Phú Thành — 2A202601289  
**Ngày:** 27/07/2026

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Đưa ra 8 vấn đề từ học tập, công việc và đời sống; chọn top 3 để phân tích | Có danh sách đủ rộng trước khi chọn giải pháp |
| Pitch Problem Card | Trình bày các vấn đề và trao đổi về bài toán tổng hợp lịch trình đa nguồn | Nhóm chọn bài toán lịch trình để đào sâu |
| Challenge bài của bạn khác | Đóng góp ý kiến và phản biện trong thảo luận | Giúp nhóm nhìn thêm rủi ro, phương án không dùng AI và giới hạn của giải pháp |
| Gom trùng / cluster | Tham gia nhóm các candidate theo dạng tra cứu, kiểm tra và điều phối | Nhóm nhìn rõ sự khác nhau giữa các loại bài toán |
| Chọn candidate problem | Đóng góp ý kiến khi so sánh các candidate | Nhóm thống nhất chọn “Trợ lý tổng hợp lịch trình đa nguồn” |
| Validation / research | Tham gia trao đổi nội bộ; chưa trực tiếp phỏng vấn đúng actor hoặc thu thập log | Nhận ra evidence hiện tại chưa đủ để quyết định Go |
| Workflow nhóm | Đóng góp ý tưởng về việc AI đọc nội dung cuộc trò chuyện để nhận biết lịch hẹn | Ý tưởng được thu hẹp: chỉ xử lý nội dung người dùng chủ động chuyển tiếp và phải duyệt trước khi lưu |
| Problem Statement | Góp ý về actor, bottleneck và phạm vi bài toán | Problem Statement tập trung vào handoff từ tin nhắn sang Calendar, không còn là “trợ lý toàn năng” |
| Rule / Workflow / Agent | Tham gia phân biệt Rule kiểm tra xung đột, AI trích xuất và người dùng duyệt | Nhóm chọn Workflow thay vì Agent |
| Decision | Tham gia thảo luận nhưng nhóm chưa có baseline thật | Quyết định phù hợp hiện tại là Not Yet |
| Trình bày | Tham gia làm slide và phản biện trong phần trao đổi với nhà đầu tư | Giúp nhóm trình bày vấn đề, giải pháp và rủi ro rõ hơn |

## 2. Tôi đã dùng AI như thế nào?

Tôi tự cung cấp trải nghiệm và ý chính, sau đó dùng AI để rà cấu trúc và sắp xếp lại nội dung. Tôi đọc lại và chịu trách nhiệm về bản cuối.

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi đã điều chỉnh gì? |
|---|---|---|---|---|
| Scan | Gợi ý cách trình bày problem theo actor, pain và dấu hiệu | Giúp mở rộng danh sách và chuẩn hóa bảng scan | Một số dấu hiệu và con số ban đầu chỉ là ước lượng nhưng được viết giống dữ liệu thật | Ghi rõ số nào là giả định chưa kiểm chứng |
| Problem Card | Kiểm tra card có đủ actor, workflow, bottleneck, impact và metric không | Giúp phát hiện thiếu field và nội dung lặp | Bản đầu quá dài; có card tóm tắt lặp lại phần chi tiết | Bỏ phần lặp và giữ ba card đầy đủ |
| Workflow | Sắp xếp các bước hiện tại và tương lai | Giúp nhìn thấy vị trí Rule, AI và human boundary | Có phép tính thời gian không khớp: 150 phút không bằng tổng các bước; Card lịch trình cũng dùng hai baseline khác nhau | Sửa lại số cho nhất quán và ghi đây là baseline giả định |
| Research | Tìm giải pháp như Google Calendar, Calendly và Zapier | Cho thấy booking link và automation có thể giải một phần mà không cần Agent | Công cụ có sẵn không chứng minh pain của người dùng trong nhóm là thật | Chỉ dùng research để so sánh giải pháp, không dùng thay cho validation |
| Problem Statement | Kiểm tra sự liên kết giữa actor, workflow, bottleneck, impact, metric và boundary | Giúp thu hẹp bài toán vào bước chuyển tin nhắn sang Calendar | Ý tưởng ban đầu “duyệt tất cả cuộc trò chuyện” quá rộng và có rủi ro riêng tư | Đổi thành chỉ đọc nội dung người dùng chủ động chuyển tiếp |
| Rule / Workflow / Agent | So sánh ba mức giải pháp | Giúp nhận ra kiểm tra trùng lịch nên dùng Rule, không cần AI | Ban đầu dễ gọi toàn bộ giải pháp là trợ lý AI hoặc Agent | Chọn Workflow: AI trích xuất, Rule kiểm tra, người dùng duyệt |
| Decision | Đối chiếu evidence với điều kiện Go / Not Yet / No-Go | Giúp chỉ ra nhóm chưa có baseline, log và phỏng vấn đúng actor | AI có thể tạo một báo cáo trông hoàn chỉnh dù dữ liệu thật còn thiếu | Giữ quyết định Not Yet và viết rõ điều cần kiểm chứng |

## 3. Reflection

Khi nghe và so sánh các candidate, tôi nhận ra một vấn đề nghe hấp dẫn chưa chắc đã là vấn đề phù hợp nhất để dùng AI. Bài toán thẩm định dataset gần với trải nghiệm của học viên AI20k và dễ kiểm chứng hơn. Bài tra cứu quy chế có actor rõ nhưng FAQ hoặc search tốt hơn có thể đã giải quyết phần lớn nhu cầu. Ý tưởng lộ trình cá nhân hóa có impact lớn nhưng cần nhiều dữ liệu và quá rộng cho thời gian lab. Bài tổng hợp lịch trình được chọn vì workflow trước và sau dễ hình dung, đồng thời có thể tách rõ phần Rule, AI và con người.

Ý tưởng ban đầu của tôi là AI có thể duyệt qua tất cả cuộc trò chuyện để tìm thông tin lịch hẹn và lưu vào Calendar. Sau khi phân tích kỹ hơn, tôi thấy cách này quá rộng. Nó có thể đọc cả nội dung không liên quan, làm lộ thông tin khách hàng hoặc hiểu nhầm một câu trao đổi thành cuộc hẹn. Vì vậy, boundary hợp lý hơn là người dùng chủ động chuyển tiếp nội dung cần xử lý. AI chỉ trích xuất người, thời gian, địa điểm và mục đích; Rule kiểm tra xung đột; người dùng phải duyệt trước khi ghi lịch.

Nhóm có lúc tiến gần đến solution-first vì bắt đầu từ ý tưởng “trợ lý AI quản lý lịch”. Việc vẽ current workflow giúp tôi quay lại câu hỏi thật: người dùng đang kẹt ở bước nào? Bottleneck không phải “chưa có AI”, mà là thông tin hẹn nằm ở nhiều kênh và phải chuyển thủ công sang Calendar. Điều này cũng cho thấy booking link hoặc một form cố định có thể là phương án đơn giản hơn.

AI hỗ trợ tôi tốt ở việc rà cấu trúc bài, hệ thống hóa cuộc trao đổi và mô tả workflow. Tuy nhiên, AI cũng làm bản đầu dài, lặp nội dung và sử dụng một số con số ước lượng giống như số liệu thật. Tôi chưa tự phát hiện hết các lỗi ngay từ đầu; phần lớn được chỉ ra trong quá trình AI kiểm tra lại. Phần tôi trực tiếp xác nhận và sửa là bối cảnh AI20k, candidate nhóm chọn và thông tin thành viên. Qua đó tôi hiểu rằng không nên nhận output của AI chỉ vì nó trình bày trôi chảy. Tôi cần tự cộng lại số liệu, hỏi nguồn và phân biệt rõ quan sát với giả định.

Đóng góp thực tế của tôi là đưa ý kiến trong thảo luận, tham gia làm slide và phản biện trong phần trao đổi với nhà đầu tư. Tôi cũng góp phần làm rõ candidate lịch trình và cách AI có thể hỗ trợ. Tôi không phụ trách validation chính và nhóm chưa có phỏng vấn hoặc log đủ chắc. Vì vậy, tôi đồng ý với quyết định Not Yet thay vì cố chọn Go để bài trông hoàn chỉnh.

Điều khó nhất khi viết Problem Statement là nối metric với bằng chứng. Viết mục tiêu “giảm xuống 15 phút” khá dễ, nhưng chứng minh baseline hiện tại là bao nhiêu và cách đo mới là phần khó. Nếu chưa đo, con số chỉ là giả định. Boundary cũng quan trọng không kém metric vì giải pháp liên quan đến hội thoại và dữ liệu khách hàng.

Nếu làm lại, tôi sẽ thảo luận nhiều hơn và challenge nhóm sớm hơn ở ba điểm: pain có thật với đúng actor không, booking link có giải được phần lớn trường hợp không, và dữ liệu nào được phép đưa cho AI. Tôi cũng sẽ ghi lại câu trả lời của từng người ngay trong buổi trao đổi, thay vì chỉ nhớ rằng mọi người “đều thấy ổn”. Như vậy quyết định cuối sẽ dựa trên evidence rõ hơn.

## 4. Tôi tự giải thích mạch bài toán

```text
Problem:
Lịch hẹn đến từ nhiều kênh và phải chuyển thủ công.

→ Workflow:
Nhận tin → ghi tạm → nhập Calendar → kiểm tra trùng → rà lại.

→ Metric:
Đo thời gian xử lý, số lần trùng/sót và độ chính xác khi trích xuất.

→ Boundary:
Chỉ xử lý nội dung được chuyển tiếp; không tự đọc toàn bộ hội thoại,
không tự nhắn và không tự ghi lịch trước khi người dùng duyệt.

→ Độ phù hợp với AI:
Rule kiểm tra trường và xung đột; AI chỉ đọc hiểu tin nhắn;
Workflow nối các bước cố định; không cần Agent tự lập kế hoạch.

→ Decision:
Not Yet vì chưa có baseline, phỏng vấn đúng actor và dữ liệu kiểm thử.
```
