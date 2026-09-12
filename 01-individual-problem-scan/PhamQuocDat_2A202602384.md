# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Phạm Quốc Đạt
- Mã học viên: 2A202602384
- Vai trò / bối cảnh: Fresher Data Analyst tại một công ty E-commerce quy mô ~150 nhân sự; stack chính gồm SQL (BigQuery), Python, Power BI/Metabase, Jira và Slack.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): 
  - Tiếp nhận và xử lý các yêu cầu trích xuất dữ liệu ad-hoc (pull data) từ team Marketing và Sales qua ticket/Slack.

  - Viết câu lệnh SQL, kiểm tra tính toàn vẹn (data validation) và reconcile số liệu giữa dashboard với database gốc.

  - Tạo, bảo trì và cập nhật các báo cáo/dashboard định kỳ (Performance Dashboard, Funnel Conversion) trên Metabase/Power BI.

  - Tìm kiếm, làm rõ định nghĩa các trường dữ liệu (data dictionary/business logic) từ schema cũ hoặc hỏi senior DA.
---

## Phase 1 — Individual Problem Scan

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại | Trích xuất và format file Excel báo cáo GMV/đơn hàng cho team Marketing từ SQL query cố định mỗi sáng | Fresher DA, Marketing Ops | Mất 20-30 phút/ngày, lặp lại 5 ngày/tuần |
| 2 | Lặp lại | Viết lại các đoạn CTE/JOIN cơ bản tương tự nhau (map User ID, Transaction status, lọc test order) khi bắt đầu query mới | Fresher DA | Lặp lại 4-6 lần/ngày trong DBeaver/BigQuery console |
| 3 | Tốn thời gian | Đọc và debug một query SQL dài 150-200 dòng kế thừa từ người cũ để tìm lỗi chênh lệch số (mismatched data) | Fresher DA, Senior DA | Mất 60-90 phút/lần xử lý; gặp 2-3 lần/tuần |
| 4 | Tốn thời gian | Kiểm tra và mapping thủ công bảng danh mục sản phẩm/mã campaign không đồng nhất giữa file Google Sheets của Sales với Database | Fresher DA | Mất 45 phút/lần chuẩn hóa file, tần suất 1 lần/tuần |
| 5 | AI có thể tốt hơn | Schema database có hàng trăm bảng nhưng thiếu Data Dictionary chuẩn, phải tự đoán bảng/cột chứa chỉ số cần tính | Fresher DA, Data Team | Mất 15-20 phút/lần lục schema hoặc gõ SELECT * LIMIT 5 để kiểm tra |
| 6 | AI có thể tốt hơn | Chuyển đổi yêu cầu phân tích kinh doanh (dưới dạng văn bản mô tả logic tính) thành khung truy vấn SQL logic ban đầu | Fresher DA, Business Stakeholder | Mất 30-40 phút nháp logic trước khi viết query thật; 3-4 ticket/tuần |
| 7 | Pain từ người khác | Team Business gửi ad-hoc request mập mờ qua Slack (thiếu time range, không rõ status đơn, không rõ nhóm đối tượng) | Fresher DA, Business User | Phải chat hỏi lại 3-4 tin nhắn/request; trung bình 5 request/tuần |
| 8 | Pain từ người khác | Stakeholder báo số trên Dashboard không khớp với báo cáo nội bộ của họ nhưng không cung cấp ID đơn hoặc snapshot mẫu | Fresher DA, Stakeholder, Data Lead | Tốn 2-3 tiếng/lần verify và trả lời ticket "Số bị sai" |
| 9 | Tốn thời gian | Viết tóm tắt diễn giải ý nghĩa số liệu (Data Insight Summary) bằng lời vào slide thuyết trình sau khi vẽ xong dashboard | Fresher DA, Line Manager, Biz Lead | Mất 45-60 phút/dashboard sprint; hay bị sửa lại cách dùng từ |
| 10 | Lặp lại | Chụp màn hình các chart từ Metabase rồi paste vào Slack channel nội bộ để thông báo kết quả campaign định kỳ | Fresher DA, Product Team | Mất 15 phút/lần, lặp lại 2-3 lần/tuần |

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Đóng vai trò Fresher Data Analyst làm việc với SQL, Metabase, Jira và Stakeholder; hãy gợi ý các tác vụ hàng ngày gặp vấn đề về lặp lại, tốn thời gian, pain point giao tiếp và điểm AI có thể hỗ trợ.
- Ý dùng được: Các vấn đề về truy vấn SQL lặp lại, debug logic kế thừa từ người cũ, thiếu hụt data dictionary, và khâu clarify yêu cầu ad-hoc còn lỏng lẻo từ stakeholder.
- Ý bỏ vì không phải pain thật: "Tự động hóa hoàn toàn việc đưa ra quyết định kinh doanh thay CEO" (không thực tế với Fresher DA, phạm vi quá lớn). "AI tự viết model Machine Learning dự báo doanh thu" (Fresher DA chủ yếu làm BI/reporting và data pull, hiếm khi train predictive model phức tạp).

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Team Business gửi ad-hoc request mập mờ qua Slack | Workflow rõ ràng; lặp lại hàng tuần; bottleneck giao tiếp làm nghẽn tiến độ; impact đo đếm được qua số ping/thời gian chờ | Business user có sẵn sàng điền theo form chuẩn/trả lời câu hỏi bot không |
| 2 | Đọc và debug một query SQL dài 150-200 dòng kế thừa từ người cũ để tìm lỗi chênh lệch số | Pain point thực tế của Fresher; tốn nhiều thời gian phân tích logic; AI xử lý đọc hiểu SQL rất tốt | Khó khăn khi SQL query phụ thuộc vào business logic ngầm ngoài database |
| 3 | Chuyển đổi yêu cầu phân tích kinh doanh thành khung truy vấn SQL logic ban đầu | AI phát huy mạnh năng lực Text-to-SQL; giảm thời gian chuyển đổi context từ Biz sang Tech; dễ scale | Rủi ro AI hallucinate sai tên cột/bảng nếu không có schema context đầy đủ |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Xử lý Ad-hoc Data Request mập mờ qua Slack

```text
Problem 1 câu:
Fresher DA mất nhiều thời gian qua lại trên Slack để làm rõ các yêu cầu trích xuất dữ liệu ad-hoc thiếu ngữ cảnh từ team Business, khiến việc chốt spec bị kéo dài và trễ hạn bàn giao data.

Actor:
Fresher Data Analyst và Business Stakeholder (Marketing/Sales Ops).

Thời điểm / bối cảnh:
Giữa tuần khi các team Business chuẩn bị chạy chiến dịch hoặc họp review tuần và cần số liệu gấp.

Current workflow 3-7 bước:
1. Nhận tin nhắn request trích xuất data từ Business qua kênh Slack.
2. Đọc và phát hiện thiếu thông tin (thiếu time range, logic lọc đơn, nhóm user).
3. Chat qua lại trên Slack để hỏi và làm rõ từng tiêu chí.
4. Chốt logic cuối cùng và xác nhận lại với Business.
5. Viết câu truy vấn SQL để lấy dữ liệu.
6. Export file kết quả và gửi lại qua Slack.

Bottleneck:
Bước 3 — Chat qua lại để làm rõ yêu cầu mất khoảng 30-45 phút chờ phản hồi và dễ hiểu lầm ý nhau.

Impact:
Fresher DA nhận trung bình 5 request/tuần, mất từ 2.5 - 3.5 giờ/tuần chỉ để nhắn tin làm rõ spec. Toàn bộ quy trình trả data bị trễ 2-4 tiếng, ảnh hưởng đến tiến độ ra quyết định của Business.

Success metric:
Giảm số lượt trao đổi làm rõ từ 3-4 tin nhắn xuống còn 1 lần xác nhận; rút ngắn thời gian chốt spec từ 45 phút xuống dưới 10 phút/request.

Non-AI alternative:
Tạo template Google Form / Jira Ticket bắt buộc điền các trường; tuy nhiên Business thường bỏ qua vì tốn công, vẫn nhắn trực tiếp qua Slack.

AI hypothesis:
AI tự động phân tích tin nhắn Slack thô của Business, đối chiếu với checklist đầu vào chuẩn (time range, metric, filter), và tạo ngay bản nháp spec kèm câu hỏi gợi ý các điểm còn thiếu để hai bên xác nhận nhanh.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

**Draft workflow Card #1:**

CURRENT STATE — 75 phút

[1 Nhận message: 5'] 
→ [2 Đọc & check thiếu: 10'] 
→ [3 Chat qua lại làm rõ: 35'] <-- bottleneck 
→ [4 Chốt spec: 5'] 
→ [5 Viết SQL: 15'] 
→ [6 Export & gửi: 5']

FUTURE STATE — 32 phút

[1 AI parse message & list điểm thiếu: 1'] 
→ [2 DA duyệt câu hỏi & gửi form chốt spec: 2'] 
→ [3 Business confirm: 5'] 
→ [4 DA review & chốt logic: 4'] <-- human boundary 
→ [5 Viết SQL: 15'] 
→ [6 Export & gửi: 5']

Fallback: nếu AI parse sai ngữ cảnh kinh doanh → DA trực tiếp gọi điện hoặc nhắn tin trao đổi lại theo checklist thủ công.

---

#### Problem Card #2 — Debug Query SQL dài kế thừa từ người cũ

```text
Problem 1 câu:
Fresher DA mất từ 60-90 phút để đọc hiểu và truy vết lỗi logic trong các câu lệnh SQL phức tạp (150-200 dòng, nhiều CTE lồng nhau) kế thừa từ nhân sự cũ khi xảy ra lệch số trên báo cáo.

Actor:
Fresher Data Analyst, Senior Data Analyst (reviewer/escalation).

Thời điểm / bối cảnh:
Khi dashboard định kỳ bị sai lệch số liệu hoặc stakeholder phản ánh số không khớp giữa hai báo cáo, cần DA điều tra nguyên nhân gốc (root cause).

Current workflow 3-7 bước:
1. Nhận thông báo lỗi lệch số từ dashboard hoặc stakeholder.
2. Mở file SQL cũ (150-200 dòng gồm 5-7 bảng CTE lồng nhau).
3. Đọc hiểu luồng xử lý và bóc tách từng đoạn CTE ra chạy thử riêng lẻ.
4. Đối chiếu logic JOIN, điều kiện WHERE và GROUP BY để tìm điểm làm nhân đôi dòng hoặc sót dữ liệu.
5. Sửa lỗi logic, kiểm tra lại tổng số và commit phiên bản query mới.

Bottleneck:
Bước 3 & 4 — Bóc tách và đọc hiểu logic từng CTE lồng nhau không có comment giải thích mất khoảng 45-60 phút.

Impact:
Xảy ra 2-3 lần/tuần, tiêu tốn khoảng 3-4.5 giờ/tuần của Fresher DA; làm kéo dài thời gian sửa lỗi dashboard (MTTR) từ nửa ngày đến một ngày làm việc.

Success metric:
Rút ngắn thời gian đọc hiểu và định vị lỗi logic từ 60-90 phút xuống dưới 25 phút/lần debug.

Non-AI alternative:
Viết tài liệu Data Lineage và bắt buộc thêm comment giải thích vào query khi bàn giao; giải pháp này khó áp dụng ngược cho hàng trăm query cũ đã chạy ngầm trong hệ thống.

AI hypothesis:
AI nhận đầu vào là đoạn SQL dài kèm thông tin chênh lệch số, tự động phân rã cây phụ thuộc (DAG của CTEs), tóm tắt logic từng bước và chỉ ra các điểm rủi ro tiềm ẩn (như Cartesian JOIN, lọc sai NULL, gộp điều kiện AND/OR sai).

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

**Draft workflow Card #2:**

CURRENT STATE — 80 phút

[1 Nhận alert lệch số: 5'] 
→ [2 Đọc hiểu SQL cũ: 25'] 
→ [3 Bóc tách & test từng CTE: 30'] <-- bottleneck 
→ [4 Tìm ra bug logic: 10'] 
→ [5 Fix & test lại số: 10']

FUTURE STATE — 23 phút

[1 Nhận alert & input SQL vào AI: 2'] 
→ [2 AI phân rã CTE & highlight rủi ro logic: 1'] 
→ [3 DA review điểm nghi vấn AI chỉ ra: 10'] <-- human boundary 
→ [4 DA fix lỗi & test lại số: 10']

Fallback: nếu AI phân tích sai cấu trúc CTE → DA quay lại phương pháp bóc tách chạy thử từng bảng tạm như quy trình thủ công.

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Chuyển đổi Business Request thành khung truy vấn SQL logic

```text
Problem 1 câu:
Fresher DA mất từ 30-45 phút để chuyển đổi yêu cầu phân tích kinh doanh trừu tượng thành logic truy vấn SQL chuẩn xác (xác định bảng nguồn, điều kiện lọc, logic JOIN), dễ dẫn đến sai sót logic ngay từ bước phác thảo ban đầu.

Actor:
Fresher Data Analyst, Business Stakeholder (Product/Marketing).

Thời điểm / bối cảnh:
Khi nhận được ticket yêu cầu phân tích hoặc tính toán chỉ số mới (ví dụ: Retention rate theo cohort, Funnel drop-off) cần viết truy vấn từ đầu.

Current workflow 3-7 bước:
1. Đọc văn bản yêu cầu và bóc tách các metrics/dimensions cần tính.
2. Tra cứu cấu trúc database để xác định các bảng và cột liên quan.
3. Nháp logic nối bảng (JOIN conditions) và bộ lọc điều kiện (WHERE/HAVING) ra giấy hoặc text editor.
4. Viết khung câu lệnh SQL hoàn chỉnh vào công cụ query (DBeaver/BigQuery).
5. Chạy thử với tập dữ liệu nhỏ (LIMIT 100) để kiểm tra logic đầu ra.

Bottleneck:
Bước 3 — Nháp logic nối bảng và điều kiện lọc đa chiều mất 20-25 phút do phải suy luận ngữ cảnh kinh doanh sang cú pháp kỹ thuật.

Impact:
Fresher DA xử lý 3-4 ticket loại này mỗi tuần, tốn khoảng 2-3 giờ chỉ cho khâu nháp logic khung; nếu nháp sai logic ngay từ đầu thì công sức viết và sửa lại query sau đó có thể tốn gấp đôi.

Success metric:
Rút ngắn thời gian từ lúc nhận yêu cầu đến khi có bản SQL draft hợp lệ từ 40 phút xuống dưới 15 phút; giảm tỷ lệ phải đập đi viết lại cấu trúc query chính.

Non-AI alternative:
Tạo thư viện mẫu SQL snippets (Query templates) cho các tác vụ phổ biến; tuy nhiên template tĩnh khó tùy biến linh hoạt theo các yêu cầu kinh doanh biến động liên tục.

AI hypothesis:
AI nhận đầu vào là mô tả yêu cầu kinh doanh bằng ngôn ngữ tự nhiên kèm schema thông tin bảng liên quan, tự động sinh ra bản thảo truy vấn SQL (draft query) chuẩn cú pháp kèm chú thích logic từng bước để DA kiểm tra.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

**Draft workflow Card #3:**

CURRENT STATE — 45 phút

[1 Đọc & bóc tách metric: 5'] 
→ [2 Tra cứu schema bảng: 10'] 
→ [3 Nháp logic JOIN & Filter: 20'] <-- bottleneck 
→ [4 Viết SQL draft: 7'] 
→ [5 Chạy test mẫu nhỏ: 3']

FUTURE STATE — 14 phút

[1 Input request + schema vào AI: 2'] 
→ [2 AI gen SQL draft & giải thích logic: 1'] 
→ [3 DA review logic & chỉnh sửa syntax: 8'] <-- human boundary 
→ [4 Chạy test mẫu nhỏ: 3']

Fallback: nếu AI sinh logic query sai lệch so với business rule → DA lấy lại cấu trúc bảng đã gợi ý và tự viết lại logic thủ công theo cách truyền thống.

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**
```text
Problem Card #1 — Xử lý Ad-hoc Data Request mập mờ qua Slack

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Đây là workflow tiếp nhận yêu cầu trích xuất dữ liệu ad-hoc xảy ra hàng tuần giữa Fresher DA và team Business (Marketing/Sales Ops). Nút thắt lớn nhất nằm ở khâu chat qua lại 3-4 tin nhắn để làm rõ các tiêu chí thiếu (time range, filter logic), làm mất 30-45 phút mỗi request và làm chậm tiến độ bàn giao data từ 2-4 tiếng. Giải quyết bài này bằng AI parsing sẽ trực tiếp cắt giảm hơn 50% thời gian chốt spec, giải phóng 2.5-3.5 giờ/tuần cho DA và giúp các bên kinh doanh nhận số liệu đúng hạn để ra quyết định.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Nếu Business user vẫn giữ thói quen nhắn tin tự do cực ngắn (ví dụ: "kéo giúp anh số tuần này") mà không chịu đọc bản checklist phản hồi từ AI/bot thì giải pháp này có bị gãy không?
2. Khi business logic có những định nghĩa ngầm (ví dụ: "đơn hợp lệ" loại trừ tài khoản nội bộ nào) mà schema database không thể hiện thì làm sao đảm bảo AI không parse thiếu hoặc hiểu sai?
```

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
