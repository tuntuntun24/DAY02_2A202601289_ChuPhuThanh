# Group Report — Day 02

## Thành viên nhóm

| STT |    Họ và tên    | Mã học viên | Vai trò trong nhóm |
|-----|-----------------|-------------|--------------------|
|  1  |  Chu Phú Thành  | 2A202601289 |    Thành viên    |
|  2  |  Vũ Thành Dương | 2A202602007 |    Thành viên    |
|  3  |  Lê Thành Nam   | 2A202601397 |    Nhóm trưởng   |
|  4  |  Phạm Thế Trung | 2A202601299 |    Thành viên    |

## 1. Group convergence

### Nhật ký hội tụ

Bảng dưới tổng hợp bốn candidate chính được các thành viên đưa ra trong phần thảo luận nhóm.

| Người đưa ra | Candidate problem | Actor | Bottleneck | Cảm nhận nhanh |
|---|---|---|---|---|
| Chu Phú Thành | Thẩm định dataset cho project ML | Học viên AI20k làm project ML | Kiểm chất lượng thủ công và tìm lại khi dataset không phù hợp | Dễ kiểm chứng trong lớp, nhưng phạm vi hẹp |
| Lê Thành Nam | Tra cứu quy chế cho sinh viên năm nhất | Sinh viên; cố vấn và ban cán sự | Tài liệu phân tán; câu trả lời trong group bị trôi | Pain dễ hiểu, nhưng FAQ có thể đã đủ |
| Vũ Thành Dương | Tổng hợp lịch trình đa nguồn | Chủ doanh nghiệp nhỏ hoặc quản lý không có trợ lý | Chuyển lịch hẹn từ nhiều kênh vào calendar và phát hiện xung đột muộn | Workflow và ranh giới người–máy rõ |
| Phạm Thế Trung | Xây dựng lộ trình cá nhân hóa theo năng lực | Sinh viên cần chọn môn học hoặc định hướng phát triển | Thiếu cách nối năng lực hiện tại, mục tiêu và các bước học phù hợp | Impact tiềm năng lớn nhưng phạm vi và dữ liệu đầu vào rộng |

### Cluster

| Cluster | Candidates included | Pattern chung |
|---|---|---|
| Kiểm tra và ra quyết định | Thẩm định dataset | Đọc nhiều thông tin trước khi chốt lựa chọn |
| Tra cứu thông tin | Quy chế sinh viên | Tìm câu trả lời trong nguồn dài, phân tán |
| Điều phối công việc | Tổng hợp lịch trình | Chuyển thông tin giữa nhiều kênh và kiểm tra xung đột |
| Cá nhân hóa và lập kế hoạch | Lộ trình theo năng lực | Đánh giá hiện trạng để đề xuất chuỗi bước phù hợp với từng người |

### Shortlist và chấm điểm

Điểm 1–5 dưới đây là công cụ hội tụ tạm thời, không phải kết quả đo người dùng.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Tổng hợp lịch trình đa nguồn | 5 | 5 | 2 | 4 | 5 | 5 | 4 | 30 |
| Thẩm định dataset | 4 | 5 | 3 | 4 | 5 | 5 | 3 | 29 |
| Tra cứu quy chế | 4 | 4 | 2 | 3 | 4 | 4 | 3 | 24 |

**Candidate nhóm chọn:** Trợ lý tổng hợp lịch trình đa nguồn.

**Vì sao chọn:**

- Luồng hiện tại có các bước và điểm bàn giao rõ.
- Có thể đo thời gian quản lý lịch và số lần trùng/sót hẹn.
- Có thể phân tách Rule, AI Workflow và phần con người duyệt.
- Bài toán đủ hẹp nếu chỉ xử lý nội dung được chủ động chuyển tiếp.

**Vì sao không chọn các candidate còn lại:**

- Thẩm định dataset dễ validate nhưng actor hẹp và có nguy cơ gộp hai pain: tìm dataset và kiểm định dataset.
- Tra cứu quy chế có actor rõ nhưng FAQ, mục lục và search truyền thống có thể giải phần lớn câu hỏi; tính hiệu lực của tài liệu cũng chưa được kiểm tra.
- Lộ trình cá nhân hóa có impact tiềm năng lớn nhưng quá rộng cho một buổi lab; cần dữ liệu năng lực, mục tiêu, chương trình học và tiêu chí đánh giá chất lượng lộ trình.

**Xử lý khác biệt ý kiến:** Nhóm dùng điểm số để mở thảo luận, sau đó ưu tiên candidate có workflow trước/sau và boundary rõ. Điểm số không tự quyết định kết quả.

## 2. Quick validation

Kết quả hiện có mới là tín hiệu từ thảo luận nội bộ; nhóm chưa có phỏng vấn đúng actor hoặc log để coi là validation hoàn tất.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Thảo luận nội bộ | 4 thành viên | Nhiều nguồn lịch làm tăng thao tác chuyển thông tin; phát hiện trùng muộn gây khó xử | Có thể yêu cầu mọi người dùng booking link, không cần AI | Thu hẹp vào cuộc hẹn vẫn đến qua tin nhắn/email |
| Desk research | 4 nguồn online | Có sẵn booking page, chuyển email thành event và workflow kết nối Calendar | Nguồn online chứng minh giải pháp tồn tại, không chứng minh actor của nhóm có pain | Giữ research tách biệt với bằng chứng người dùng |
| Phỏng vấn đúng actor | 0 | Chưa có | Chưa biết pain có đủ lớn không | Không dùng số ước lượng như dữ liệu thật |
| Log lịch/tin nhắn | 0 mẫu | Chưa có | Chưa biết AI trích xuất đủ chính xác không | Đặt yêu cầu pilot trên dữ liệu đã ẩn thông tin nhạy cảm |

### Kế hoạch validation tối thiểu

1. Phỏng vấn 3 chủ doanh nghiệp nhỏ hoặc quản lý tự quản lý lịch.
2. Ghi lần gần nhất họ bị sót/trùng hẹn, các kênh nhận lịch và thời gian xử lý một ngày.
3. Xin 30–50 tin nhắn đã ẩn dữ liệu cá nhân để kiểm tra bốn trường: người, thời gian, địa điểm và mục đích.
4. So sánh với phương án chỉ dùng một booking link.

## 3. Research giải pháp hiện có

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Google Calendar Appointment Schedules | [Google Calendar Help](https://support.google.com/calendar/answer/10729749?hl=en) | Booking page, availability, buffer và kiểm tra lịch bận | Không cần AI; tránh double-booking từ đầu | Chỉ hiệu quả khi khách dùng booking link | Pilot No-AI trước |
| Gmail → Calendar | [Google Calendar Help](https://support.google.com/calendar/answer/13469141?hl=en) | Chuyển email thành Calendar event để người dùng xác nhận | Có sẵn; người dùng vẫn kiểm soát | Chỉ bao phủ email | Pattern phù hợp là draft rồi duyệt |
| Calendly Availability | [Calendly](https://calendly.com/scheduling/availability) | Chia sẻ thời gian rảnh, kiểm tra lịch và tự ghi booking | Mạnh ở tránh double-booking | Đòi hỏi đối tác dùng booking page | Có thể giải phần lớn case không cần AI |
| Zapier Gmail + Google Calendar | [Zapier](https://zapier.com/apps/gmail/integrations/google-calendar/10363/create-google-calendar-events-from-new-gmail-emails) | Tạo Calendar event từ email theo trigger | Điều phối rõ, cấu hình được trường event | Mapping sai có thể tạo lịch sai; chưa xử lý mọi kênh | Chỉ tự động hóa sau bước duyệt |

**Research takeaway:** Công cụ có sẵn xử lý tốt booking link hoặc email, nhưng chưa giải trọn việc gom cuộc hẹn không cấu trúc từ nhiều kênh. Hướng phù hợp là Workflow có AI trích xuất, Rule kiểm xung đột và con người duyệt; chưa cần Agent tự nhắn hoặc tự đàm phán.

## 4. Workflow hiện tại

Các số trong dấu `‹ ›` là ước lượng nhóm đánh giá hợp lý sau thảo luận và desk research, chưa phải baseline đã đo.

| Bước | Actor | Input | Output | Handoff | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|---|
| 1. Nhận yêu cầu hẹn | Chủ doanh nghiệp/quản lý | Zalo, email, FB, điện thoại | Nội dung hẹn rời rạc | Sang note hoặc trí nhớ | Xen kẽ trong ngày | Không có nơi tiếp nhận chung |
| 2. Ghi nhớ hoặc ghi tạm | Chủ doanh nghiệp/quản lý | Nội dung hẹn | Note/giấy hoặc trí nhớ | Sang Calendar | ‹5 phút/ngày› | Điểm có thể sót đầu tiên |
| 3. Nhập vào Calendar | Chủ doanh nghiệp/quản lý | Note và tin nhắn | Calendar event | Sang bước kiểm tra lịch | ‹20–30 phút/ngày› | Bottleneck thao tác |
| 4. Xử lý trùng | Chủ doanh nghiệp/quản lý | Event mới và lịch hiện có | Lịch điều chỉnh | Nhắn lại đối tác nếu cần | ‹15 phút/ngày› | Phát hiện sau khi đã nhận lời |
| 5. Rà lịch ngày sau | Chủ doanh nghiệp/quản lý | Calendar | Danh sách lịch trong ngày | Sang khâu chuẩn bị cuộc hẹn | ‹15 phút/ngày› | Chuẩn bị tài liệu/di chuyển |

```text
CURRENT — ước lượng ban đầu 55–65 phút/ngày

[Nhận hẹn từ 4 kênh]
→ [Ghi nhớ/note: 5']
→ [Nhập Calendar: 20–30']          <-- bottleneck
→ [Kiểm tra trùng + nhắn dời: 15'] <-- phát hiện muộn
→ [Rà lịch sáng hôm sau: 15']
```

**Bottleneck chính:** Handoff từ tin nhắn rời rạc sang Calendar. Mỗi lần chuyển tay có nguy cơ thiếu người, thời gian, địa điểm hoặc mục đích; xung đột chỉ được phát hiện sau khi đã nhận lời.

## 5. Workflow tương lai

```text
FUTURE — mục tiêu dưới 15 phút/ngày

[Người dùng chủ động chuyển tiếp nội dung hẹn vào một inbox]
→ [AI trích xuất người / thời gian / địa điểm / mục đích]
→ [Rule kiểm tra trường bắt buộc, lịch bận và thời gian di chuyển]
→ [Hệ thống tạo thẻ nháp + cảnh báo xung đột]
→ [Người dùng sửa và duyệt]        <-- human boundary
→ [Workflow ghi Calendar + đặt nhắc lịch]

Fallback:
- Thiếu/mâu thuẫn thông tin → không tạo event, yêu cầu điền tay.
- AI lỗi → quay về form bốn trường hoặc nhập Calendar thủ công.
```

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 6 | Thêm bước duyệt để kiểm soát chất lượng |
| Tổng thời gian | Ước lượng ‹55–65 phút/ngày› | Dưới ‹15 phút/ngày› | Cần đo baseline trước pilot |
| Bước thủ công chính | 5/5 | 2/6 | Chuyển tiếp và duyệt |
| Bottleneck | Nhập tay, phát hiện trùng muộn | Review trường hợp mơ hồ | Bottleneck mới chấp nhận được |
| Risk mới | Sót do chuyển tay | AI trích sai, lộ dữ liệu | Cần review và giới hạn dữ liệu |

## 6. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Chủ doanh nghiệp nhỏ hoặc quản lý có lịch hẹn đến từ nhiều kênh, tự quản lý lịch và không có trợ lý |
| **Workflow** | Nhận hẹn → ghi tạm → nhập Calendar → kiểm tra trùng → rà lịch |
| **Bottleneck** | Chuyển thông tin thủ công vào Calendar; xung đột được phát hiện muộn |
| **Impact** | Ước lượng ‹55–65 phút/ngày› và ‹2–3 lần trùng/sót/tháng›; chưa kiểm chứng bằng log |
| **Success Metric** | Dưới ‹15 phút/ngày›; tối đa ‹0–1 lần trùng/sót/tháng›; mục tiêu trích đúng đủ bốn trường ở ≥‹90%› mẫu |
| **Boundary** | Chỉ đọc nội dung chủ động chuyển tiếp; không tự nhắn đối tác hoặc tự tạo event trước khi duyệt |

## 7. Rule / Workflow / Agent

**Ma trận:** Độ phức tạp cao vì có nhiều nguồn và bước; độ mơ hồ trung bình vì tin nhắn có nhiều cách diễn đạt nhưng output gồm các trường cố định. AI không cần tự quyết định mục tiêu hoặc bước tiếp theo.

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI / Process fix** | Thống nhất một kênh nhận lịch, dùng booking link và checklist rà lịch | Đối tác chấp nhận quy trình mới | Khách vẫn có thể nhắn qua kênh cũ | Pilot trước |
| **Rule** | Form bốn trường + kiểm tra lịch trùng + booking link | Đối tác chấp nhận form/link | Không xử lý tốt tin nhắn tự nhiên | Pilot đối chứng |
| **Workflow** | AI trích xuất → Rule kiểm tra → người duyệt → ghi Calendar | Các bước và quyền quyết định cố định | AI trích sai; dữ liệu riêng tư | **Chọn có điều kiện** |
| **Agent** | Tự đọc inbox, đàm phán và nhắn đối tác | Khi thật sự cần tự chọn hành động nhiều vòng | Nhắn/đặt sai lịch, vượt quyền; khó rollback | Không chọn |

**Mức chọn:** Workflow.

**Vì sao:** Tin nhắn cần khả năng đọc hiểu, nhưng các bước sau có thứ tự cố định. Rule kiểm tra trường bắt buộc và xung đột; người dùng giữ quyền duyệt.

**Vì sao không chỉ dùng Rule:** Rule/booking link phải được pilot trước và có thể giải phần lớn trường hợp. AI chỉ đáng thêm nếu nhiều cuộc hẹn vẫn đến bằng tin nhắn tự nhiên và người dùng không thể ép đối tác đổi kênh.

## 8. Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Chủ doanh nghiệp nhỏ hoặc quản lý tự quản lý lịch, nhận cuộc hẹn qua ít nhất ba kênh |
| **Workflow** | Nhận tin → ghi tạm → nhập Calendar → kiểm tra xung đột → điều chỉnh → rà lịch |
| **Bottleneck** | Chuyển tay thông tin không cấu trúc vào Calendar và phát hiện xung đột sau khi nhận lời |
| **Impact** | Có nguy cơ tốn thời gian và ảnh hưởng uy tín khi sót/trùng; mức cụ thể chưa đo |
| **Success Metric** | Đo baseline 2 tuần; pilot hướng tới giảm ≥50% thời gian, không quá 1 sự cố/tháng và ≥90% mẫu trích đủ bốn trường |
| **Boundary** | Chỉ xử lý nội dung chủ động chuyển tiếp; không quét inbox; không tự nhắn; không tự ghi Calendar |
| **AI intervention point** | Trích xuất bốn trường và tạo thẻ nháp |
| **Mức chọn** | Workflow |
| **Rủi ro & người thật kiểm tra** | AI có thể hiểu sai/lộ dữ liệu; chủ lịch phải review trước khi lưu |

## 9. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor và workflow đã rõ chưa? | Yes | Đã thu hẹp actor và mô tả từng bước |
| Baseline và success metric đã đo chưa? | Not Yet | Các số hiện tại là giả định |
| Có data/input đủ dùng chưa? | Not Yet | Chưa có tập tin nhắn đã ẩn dữ liệu |
| Nếu AI sai, hậu quả chấp nhận được không? | Not Yet | Chỉ chấp nhận nếu duyệt trước khi lưu |
| Có người review/owner không? | Yes | Chủ lịch duyệt và chịu trách nhiệm |
| Có cách non-AI đơn giản hơn không? | Yes | Booking link, form và Rule kiểm xung đột |

**Decision: NOT YET**

**Lý do:** Workflow và boundary đã rõ, nhưng nhóm chưa có baseline thật, phỏng vấn đúng actor hoặc tập mẫu kiểm tra độ chính xác. Quyết định Go lúc này sẽ dựa trên giả định.

**Cần validate trước:**

1. Đo workflow của ít nhất 3 actor trong 2 tuần.
2. Pilot booking link/form để biết No-AI giải được bao nhiêu trường hợp.
3. Kiểm thử AI trên 30–50 tin nhắn đã ẩn dữ liệu.
4. Chỉ Go nếu AI tạo thêm giá trị rõ so với Rule và bước duyệt kiểm soát được rủi ro.

**Pilot nhỏ nhất sau khi đạt điều kiện:** Người dùng tự dán nội dung vào form; hệ thống chỉ tạo thẻ nháp và cảnh báo xung đột. Chưa kết nối trực tiếp Zalo/FB/email và chưa tự ghi Calendar.
