# 01 — Individual Problem Scan

**Học viên:** Chu Phú Thành — 2A202601289  
**Ngày:** 27/07/2026

> **Trạng thái dữ liệu:** Các số trong dấu `‹ ›` là giả định ban đầu chưa kiểm chứng, không phải baseline thực tế.

## Phase 1 — Bảng scan (8 problems)

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian · AI có thể tốt hơn | Chọn mua laptop giữa quá nhiều mẫu mã, không biết cấu hình nào đủ dùng cho ngành mình sắp học | Học sinh cấp 3 vừa thi xong THPT và phụ huynh | Mỗi mùa nhập học nhóm tư vấn/FB tràn bài "ngân sách X mua máy nào"; một người mất ‹3-5 ngày› đọc review, hỏi ‹4-6› người rồi vẫn chọn theo cảm tính. Chọn sai → dùng 4 năm với máy yếu hoặc thừa tiền ‹5-10 triệu› |
| 2 | AI có thể tốt hơn · Lặp lại | Tìm và thẩm định dataset cho project ML: không biết dataset nào phù hợp và đáng tin | Học viên AI20k trong chương trình AI in Action do Vingroup và VinUniversity triển khai | Tôi đã trực tiếp trải qua các bước tìm, tải thử và kiểm dataset. Chưa có checklist chung; thời gian ‹2-3 giờ› và thiệt hại ‹2-3 ngày› nếu đổi data sau khi train là giả định cần đo |
| 3 | Lặp lại · Pain từ người khác | Thắc mắc về quy chế, thủ tục, học phí nhưng tài liệu phân tán và quá dài → mất nhiều thời gian tra cứu, cuối cùng vẫn phải hỏi người | Sinh viên năm nhất (‹8› tuần đầu); người bị hỏi lại: cố vấn học tập, ban cán sự, anh chị khóa trên | Group FB/Zalo lớp lặp lại cùng một câu hỏi mỗi tuần. Sổ tay sinh viên ‹~80› trang PDF, không search theo ngữ nghĩa được. Hỏi trong group phải chờ ‹30 phút – vài giờ› mới có người rảnh trả lời |
| 4 | Tốn thời gian · Lặp lại | Lịch hẹn đến từ Zalo / email / FB / điện thoại, phải tự tổng hợp và nhập tay vào calendar | Chủ doanh nghiệp nhỏ hoặc quản lý không có trợ lý riêng | Giả định cần phỏng vấn: ‹5-15› cuộc hẹn/tuần, ‹55-65 phút/ngày› để ghi tạm, nhập và rà lịch, sót/trùng ‹2-3 lần/tháng› |
| 5 | AI có thể tốt hơn | Chọn môn học / định hướng ngành theo cảm tính, không khớp năng lực thực tế và mục tiêu nghề nghiệp | Sinh viên đại học, rõ nhất là năm nhất trước kỳ đăng ký tín chỉ | Mỗi kỳ đăng ký đều có sinh viên đổi ngành/rớt môn vì chọn sai. Tư vấn hiện tại là hỏi anh chị khóa trên — mỗi người nói một kiểu. Hậu quả trễ 1 kỳ = ‹~1 học kỳ học phí› |
| 6 | Tốn thời gian · Lặp lại | Tìm quán ăn phải mở từng group FB, đọc thủ công từng bài review, không lọc được theo món / khu vực / tầm giá | Dân cư trong khu vực, sinh viên ở trọ | Mỗi lần quyết định ăn gì mất ‹10-20 phút› scroll ‹3-5› group. Bài review trôi rất nhanh, hỏi lại thì lặp câu hỏi cũ. Tần suất cao: ‹gần như hằng ngày› |
| 7 | Lặp lại · Pain từ người khác | Thông tin lớp (deadline, cách nộp bài, quyết định, link tài liệu) trôi trong Discord | Học viên AI in Action; TA và bạn học phải trả lời lại | Có log Discord để kiểm chứng; hiện ước lượng ‹5-10› câu hỏi trùng/tuần và ‹5-15 phút› mỗi lần tra |
| 8 | Lặp lại | Nộp bài lab bị thiếu file hoặc sai cấu trúc/quy ước đặt tên, chỉ phát hiện khi bị nhắc | Học viên nộp bài theo repo cá nhân mỗi ngày lab | Chính repo Day02 này quy định cấu trúc 3 thư mục + prefix đặt tên file phụ; rất dễ nộp thiếu file hoặc sai prefix. Sửa lại sau deadline có thể bị trừ điểm. Lặp lại mỗi ngày lab |

**Tổng: 8 problems**, vượt mức tối thiểu 5 problems.

---

## Phase 2 — Chọn top 3

### Bảng chọn

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | **#2 — Thẩm định dataset cho project ML** | Tôi và các học viên AI20k có thể validate ngay; workflow rõ và có thể so sánh Rule với Workflow | Chưa biết pain có phổ biến không và bottleneck nằm ở khâu tìm hay thẩm định |
| 2 | **#3 — Tra cứu quy chế / thủ tục cho sinh viên năm nhất** | Actor rõ và có 2 phía cùng chịu ảnh hưởng. Rule/FAQ có thể đã đủ nên phù hợp để so sánh với Workflow | Chưa rõ quyền sử dụng tài liệu và tỉ lệ câu hỏi trùng lặp |
| 3 | **#4 — Trợ lý tổng hợp lịch trình đa nguồn** | Workflow điều phối đa nguồn rõ và có ranh giới người–máy đáng phân tích | Khó phỏng vấn đúng actor trong thời gian lab; có rủi ro riêng tư |

---

## Problem Card #1 — Thẩm định dataset cho project ML

**Problem 1 câu:** Học viên AI20k có thể mất ‹130 phút› để tìm và thẩm định dataset cho một project ML nhưng vẫn có nguy cơ chọn dataset nhãn ẩu, sai nguồn gốc hoặc không phù hợp về license.

**Actor:** Học viên AI20k trong chương trình AI in Action do Vingroup và VinUniversity triển khai, đang tự làm project ML và chưa có nhiều kinh nghiệm đánh giá nguồn dữ liệu.

**Thời điểm / bối cảnh:** Tuần đầu tiên của một project mới — vừa chốt đề tài, cần data để bắt đầu train.

**Current workflow (6 bước):**

1. Gõ từ khóa lên Google / Kaggle / HuggingFace / Papers with Code — ‹15'›
2. Mở 5-10 tab, đọc mô tả và datacard từng dataset — ‹30'›
3. Tải thử 2-3 dataset, mở bằng pandas, xem schema / số dòng / phân bố nhãn — ‹30'›
4. **Kiểm chất lượng thủ công**: thiếu giá trị, nhãn sai, bản ghi trùng, license, nguồn gốc — ‹45'›
5. Phát hiện không dùng được (nhãn ẩu, data do model sinh ra, license cấm dùng) → **quay lại bước 1** — lặp ‹1-2› vòng
6. Chốt dataset, ghi note vào repo — ‹10'›

**Bottleneck giả định:** Bước kiểm chất lượng và vòng lặp tìm lại dataset do chưa có tiêu chí đánh giá thống nhất. Cần phỏng vấn để xác nhận bottleneck nằm ở khâu tìm candidate hay khâu thẩm định.

**Impact dự kiến:** ‹130 phút›/project; nếu chỉ phát hiện data không phù hợp sau khi train, có thể mất thêm ‹2-3 ngày›. Các số này chưa được kiểm chứng.

**Success metric:**
- Thời gian từ bắt đầu tìm đến chốt dataset kèm biên bản: baseline giả định ‹130 phút› → mục tiêu dưới ‹45 phút›
- Tỉ lệ phải đổi dataset sau khi train: baseline giả định ‹2/5 project› → mục tiêu dưới ‹1/5›
- Cách đo: bấm giờ trên 5 project; ghi ngày, lý do đổi dataset và đối chiếu commit log

**Non-AI alternative:** Checklist đánh giá dataset 10 mục + script Python tự tính missing rate, duplicate rate, class balance, có/không có trường license. Cách này giải được phần **đo đếm được** — nhưng không giải được phần **đọc hiểu** (datacard viết mơ hồ, nguồn gốc không rõ, dấu hiệu data do model sinh).

**AI hypothesis:** AI đọc datacard/README và kết quả script để lập báo cáo rủi ro có trích dẫn. Người dùng đối chiếu nguồn và quyết định cuối cùng.

**Quick gut:** `[x] Workflow` — vì các bước rõ ràng và cố định, không cần AI tự quyết định bước tiếp theo.

### Workflow trước/sau

```text
CURRENT STATE — baseline giả định 130 phút, chưa tính vòng làm lại

[Search từ khóa: 15']
→ [Đọc mô tả 5-10 tab: 30']
→ [Tải thử + xem schema: 30']
→ [Kiểm chất lượng thủ công: 45']   <-- BOTTLENECK
→ [Không dùng được: quay lại bước 1; thời gian phát sinh đo riêng]
→ [Chốt + ghi note: 10']

FUTURE STATE — mục tiêu 45 phút

[Search từ khóa: 15']
→ [Script tự chạy thống kê: missing / duplicate / class balance / license: 2']   <-- RULE
→ [AI đọc datacard + kết quả script → báo cáo rủi ro có trích dẫn: 3']           <-- AI hỗ trợ
→ [Người đọc báo cáo, đối chiếu với yêu cầu project, tự chốt: 20']               <-- HUMAN BOUNDARY
→ [Ghi biên bản kiểm chất lượng vào repo: 5']

Boundary: AI chỉ CẢNH BÁO rủi ro, KHÔNG tự loại dataset.
          License và nguồn gốc pháp lý luôn do người xác nhận lại.
Fallback: AI không đọc được datacard (thiếu/rỗng) → hạ về checklist 10 mục làm tay.
Scope: Chỉ hỗ trợ thẩm định candidate dataset đã tìm được, không giải quyết toàn bộ khâu khám phá dataset.
```

---

## Problem Card #2 — Tra cứu quy chế / thủ tục cho sinh viên năm nhất

**Problem 1 câu:** Sinh viên năm nhất mất trung bình ‹~3 giờ› để có câu trả lời cho một thắc mắc về quy chế/thủ tục, vì tài liệu chính thức dài và phân tán; đồng thời cố vấn và anh chị khóa trên phải trả lời lặp lại cùng một câu hỏi mỗi tuần.

**Actor:** Hai phía cùng đau —
- *Người hỏi:* sinh viên năm nhất, tập trung trong ‹8› tuần đầu nhập học, chưa quen hệ thống văn bản của trường.
- *Người trả lời:* cố vấn học tập, ban cán sự lớp, anh chị khóa trên — bị hỏi lặp lại.

**Thời điểm / bối cảnh:** Đầu kỳ (đăng ký tín chỉ, đóng học phí, làm thủ tục giấy tờ) và trước mỗi mốc hạn nộp.

**Current workflow (5 bước):**

1. Sinh viên gặp thắc mắc (đăng ký tín chỉ, học phí, điểm rèn luyện, xin giấy xác nhận)
2. Tìm trên website trường + sổ tay sinh viên PDF ‹~80› trang — ‹15'›
3. Không thấy, hoặc thấy bản cũ không chắc còn hiệu lực → đăng hỏi trong group FB/Zalo lớp
4. **Chờ người rảnh trả lời** — ‹30 phút đến vài giờ›
5. Có người trả lời (‹5'›/lần), câu trả lời trôi trong group → tuần sau có người hỏi lại y hệt

**Bottleneck giả định:** Hai chỗ —
- Bước 2-3: tài liệu dài, chỉ search được từ khóa chính xác, không search được theo ý nghĩa câu hỏi.
- Bước 5: **kiến thức không được tích lũy** — mỗi câu trả lời đúng đều bị mất sau vài ngày.

**Impact dự kiến:** Sinh viên chờ lâu và có nguy cơ trễ hạn thủ tục; người trả lời mất khoảng ‹5 phút› cho mỗi câu hỏi lặp. Cần đếm log nhóm lớp để xác nhận.

**Success metric:**
- Thời gian từ lúc đặt câu hỏi → có câu trả lời **kèm trích dẫn nguồn**: ‹~3h› → ‹dưới 5 phút›
- Số câu hỏi trùng lặp trong group mỗi tuần: ‹10› → ‹4› (giảm 60%)
- Tỉ lệ câu trả lời trích đúng điều/mục trong văn bản gốc: ≥ ‹90%›
- Cách đo: đếm bài đăng trong group lớp 2 tuần trước và 2 tuần sau; đối chiếu ‹30› câu hỏi mẫu với văn bản gốc

**Non-AI alternative:** FAQ 30 câu hay hỏi nhất được ghim + đánh mục lục sổ tay theo chủ đề + form gửi câu hỏi. **Cách này có thể đã giải được 70-80% case** — nhóm phải trả lời thật lòng câu hỏi này trước khi bàn đến AI.

**AI hypothesis:** RAG trên đúng tập tài liệu chính thức, mỗi câu trả lời **bắt buộc kèm trích dẫn** điều/mục và link văn bản. Câu ngoài phạm vi tài liệu → không đoán, chuyển sang người thật.

**Quick gut:** `[x] Workflow` — luồng cố định (nhận câu hỏi → tìm đoạn liên quan → trả lời kèm nguồn), không cần AI tự lập kế hoạch.

### Workflow trước/sau

```text
CURRENT STATE — baseline giả định khoảng 3 giờ/câu hỏi

[Có thắc mắc]
→ [Tra web trường + sổ tay 80 trang: 15']
→ [Không thấy / không chắc còn hiệu lực]
→ [Đăng hỏi group FB-Zalo: 2']
→ [CHỜ người rảnh: 30' – vài giờ]      <-- BOTTLENECK (thời gian chết)
→ [Anh chị trả lời: 5']
→ [Câu trả lời trôi mất]               <-- KIẾN THỨC KHÔNG TÍCH LŨY

FUTURE STATE — dưới 5 phút

[Có thắc mắc]
→ [Hỏi bằng ngôn ngữ tự nhiên: 1']
→ [Hệ thống tìm đoạn văn bản liên quan: <10s]           <-- RETRIEVAL
→ [AI trả lời KÈM trích dẫn điều/mục + link gốc: <20s]  <-- AI hỗ trợ
→ [SV đọc, bấm vào nguồn để tự xác nhận: 2']            <-- HUMAN BOUNDARY
→ [Nếu ngoài phạm vi tài liệu → chuyển cố vấn: hàng đợi] <-- ESCALATION

Boundary: CHỈ trả lời trong phạm vi văn bản đã nạp.
          KHÔNG trả lời câu hỏi về trường hợp cá nhân (điểm, hồ sơ riêng).
          Mọi câu trả lời không có trích dẫn = không được hiển thị.
Fallback: Không tìm được nguồn → nói thẳng "không có trong tài liệu"
          và chuyển cho cố vấn học tập, thay vì đoán.
```

---

## Problem Card #3 — Trợ lý tổng hợp lịch trình đa nguồn

**Problem 1 câu:** Chủ doanh nghiệp nhỏ có thể mất ‹55-65 phút› mỗi ngày để gom lịch hẹn từ ‹4› kênh vào một calendar và vẫn sót hoặc trùng ‹2-3 cuộc/tháng›.

**Actor:** Chủ doanh nghiệp vừa và nhỏ hoặc quản lý cấp trung, ‹5-15› cuộc hẹn/tuần, tự quản lý lịch, không có trợ lý riêng.

**Thời điểm / bối cảnh:** Cuối mỗi ngày làm việc (lúc ngồi nhập lịch) và sáng sớm hôm sau (lúc rà lại lịch trong ngày).

**Current workflow (5 bước):**

1. Nhận yêu cầu hẹn rải rác cả ngày: Zalo, email, tin nhắn FB, gọi điện — ‹xen kẽ trong giờ làm›
2. Tự nhớ hoặc ghi tạm vào note/giấy — **dễ sót ngay từ đây**
3. Cuối ngày mở Google Calendar nhập tay từng cuộc hẹn — ‹20-30'›
4. **Phát hiện trùng lịch hoặc không kịp di chuyển** → nhắn lại để dời hẹn — ‹15'›
5. Sáng hôm sau tự rà lại lịch, chuẩn bị tài liệu cho từng cuộc — ‹15'›

**Bottleneck:** Bước 1→3 — thông tin phân mảnh phải chuyển thủ công giữa nhiều app, mỗi lần chuyển là một cơ hội sót. Nghiêm trọng hơn: **xung đột lịch chỉ bị phát hiện ở bước 4, tức là sau khi đã nhận lời** — lúc đó chi phí sửa là phải nhắn xin lỗi và dời hẹn.

**Impact dự kiến:** ‹55-65 phút/ngày›, tương đương khoảng ‹18-22 giờ/tháng› nếu tính 20 ngày làm việc, cùng rủi ro ảnh hưởng uy tín khi sót hoặc trùng hẹn. Cần phỏng vấn để xác nhận.

**Success metric:**
- Thời gian quản lý lịch: baseline giả định ‹55-65 phút/ngày› → mục tiêu dưới ‹15 phút/ngày›
- Số lần trùng hoặc sót hẹn: ‹2-3 lần/tháng› → ‹0-1 lần/tháng›
- Tỉ lệ trích xuất đúng cả 4 trường (ai / khi nào / ở đâu / mục đích) từ tin nhắn: ≥ ‹90%›
- Cách đo: bấm giờ 2 tuần trước/sau, ghi sự cố trong một tháng và kiểm thử ‹50› tin nhắn đã ẩn dữ liệu nhạy cảm

**Non-AI alternative:** Quy ước **một kênh duy nhất** để nhận lịch và gửi booking link cho đối tác tự chọn slot. Cách này rẻ và giải quyết tận gốc, nhưng không bao phủ các trường hợp khách vẫn nhắn qua kênh quen thuộc.

**AI hypothesis:** AI đọc tin nhắn/email được chuyển tiếp vào → trích xuất (ai, khi nào, ở đâu, mục đích) → đối chiếu calendar hiện có → đề xuất slot không xung đột → **người duyệt bằng một chạm** rồi mới ghi vào calendar.

**Quick gut:** `[x] Workflow` — có thể nâng lên Agent nếu cho AI tự nhắn trả lời và đàm phán lịch, nhưng **rủi ro quá cao cho một buổi lab** (AI nhắn nhầm khách hàng là hỏng thật, không rollback được).

### Workflow trước/sau

```text
CURRENT STATE — baseline giả định 55-65 phút/ngày
                (5' ghi tạm + 20-30' nhập + 15' sửa trùng + 15' rà sáng)

[Nhận hẹn: Zalo / Email / FB / Điện thoại]  <-- 4 NGUỒN PHÂN MẢNH
→ [Ghi tạm vào note hoặc chỉ nhớ trong đầu: 5']  <-- ĐIỂM SÓT ĐẦU TIÊN
→ [Cuối ngày nhập tay từng cuộc vào Calendar: 20-30']   <-- BOTTLENECK
→ [Phát hiện trùng lịch / không kịp di chuyển: 15']     <-- PHÁT HIỆN QUÁ MUỘN
→ [Nhắn xin lỗi, dời hẹn]                               <-- CHI PHÍ UY TÍN
→ [Sáng hôm sau rà lại + chuẩn bị tài liệu: 15']

FUTURE STATE — ~15 phút/ngày

[Nhận hẹn 4 nguồn → chuyển tiếp vào 1 hộp thư chung]
→ [AI trích xuất: ai / khi nào / ở đâu / mục đích: <10s]    <-- AI hỗ trợ
→ [Rule kiểm xung đột lịch + thời gian di chuyển: <5s]      <-- RULE (tất định)
→ [Đề xuất slot thay thế nếu trùng]                         <-- CẢNH BÁO SỚM
→ [Người xem thẻ tóm tắt, duyệt 1 chạm: 10']                <-- HUMAN BOUNDARY
→ [Ghi vào Calendar + nhắc trước 1 tiếng: tự động: 0']
→ [Sáng rà lại danh sách đã duyệt: 5']

Boundary: AI KHÔNG tự trả lời hay nhắn tin cho đối tác.
          AI KHÔNG tự ghi vào calendar khi chưa được duyệt.
          Kiểm tra xung đột lịch dùng RULE (so sánh thời gian), KHÔNG dùng AI.
          Chỉ đọc tin nhắn được chủ động chuyển tiếp vào — KHÔNG quét toàn bộ hộp thư.
Fallback: AI trích xuất thiếu trường → hiện thẻ trống để người điền tay,
          vẫn nhanh hơn tự mở từng app.
Rủi ro riêng tư: tin nhắn công việc chứa thông tin khách hàng
          → phải hỏi rõ dữ liệu được lưu ở đâu, ai đọc được.
```

---

## Card tôi muốn pitch nhất

**Problem Card #1 — Thẩm định dataset cho project ML**

**Vì sao:**

- Có thể phỏng vấn ngay các học viên AI20k trong lớp.
- Tôi đã trực tiếp trải qua workflow nên mô tả được từng bước.
- Rule xử lý thống kê; AI hỗ trợ đọc datacard; người dùng quyết định cuối. Không cần Agent tự lập kế hoạch.
- Có thể đo bằng thời gian hoàn thành và số lần phải đổi dataset sau khi train.

**Câu hỏi tôi muốn nhóm challenge:**

1. Bottleneck thật nằm ở khâu tìm candidate hay khâu thẩm định?
2. Checklist và script có giải được phần lớn vấn đề mà không cần AI không?
3. AI cảnh báo sai thì ai phát hiện và hậu quả là gì?
