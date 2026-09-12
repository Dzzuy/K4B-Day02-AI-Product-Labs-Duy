# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
| -----| -----------| -------------| ------------------------------------------------------------------|
| 1 | Phạm Đình Duy | 2A202602913 | Synthesis, problem framing, learning pain |
| 2 | Bùi Văn Quang | 2A202602688 | Developer workflow, reporting/code review/test pain |
| 3 | Võ Trường An | 2A202602656 | Full-stack debug, codebase navigation, setup pain |
| 4 | Lâm Quang Anh Quân | 2A202602467 | Team coordination, task ownership, task clarity |
| 5 | Phạm Quốc Đạt | 2A202602384 | Data analyst workflow, stakeholder request, SQL pain |
| 6 | Nguyễn Hữu Chương | 2A202602601 | Campus navigation, student/guest daily pain |

**Candidate problem nhóm chọn (1 câu):**

```text
Sinh viên và khách đến VinUni gặp khó khăn khi tìm phòng học/hội trường trong tòa nhà phức tạp và tìm quán ăn phù hợp quanh Ocean Park vì thông tin indoor map và tiện nghi xung quanh bị phân tán.
```
---

## Phase 3 — Group Convergence: từ candidates cá nhân về shortlist

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Duy | Sau một ngày học AI dày đặc, sinh viên không biết phần nào đã hiểu thật và phần nào còn thiếu. | Sinh viên học lecture/lab AI | Kiến thức nằm rải ở lecture, lab, VLearn, GitHub, presentation và feedback; chưa có self-check rõ. | Rất gần bối cảnh lab hiện tại, pain thật, nhưng cần cách đo "đã hiểu" rõ hơn. |
| 2 | Duy | Tìm lại tài liệu, yêu cầu hoặc đoạn hướng dẫn giữa VLearn, GitHub và link lớp mất lâu. | Sinh viên/nhóm lab | Nguồn phân tán, không có một index nguồn chuẩn. | Rõ workflow, dễ validate, có thể chỉ cần process/index trước khi AI. |
| 3 | Duy | Nhóm lab mất thời gian vì phân công, đầu ra và trạng thái task chưa rõ. | Nhóm lab | Task thiếu owner, output, deadline nhỏ và dependency. | Trùng pattern với idea của Quân, có khả năng gom thành cluster teamwork. |
| 4 | Quang | Viết báo cáo tiến độ hằng tuần từ Jira, local file, Slack, email mất khoảng 60 phút. | Sinh viên/mentor/team lead | Viết narrative từ raw data, phải chọn highlight/risk/plan thủ công. | Metric mạnh, workflow rõ, nhưng domain hơi lệch khỏi bài học/lab của cả nhóm. |
| 5 | Quang | Review code của teammates khó vì thiếu docstring/explanation, dễ miss bug. | Reviewer, teammates, team lead | Reviewer phải đọc line-by-line để hiểu intent. | Có AI fit tốt, nhưng cần code repo thật để validate. |
| 6 | Quang | Test local fail do config environment không đồng nhất giữa máy các thành viên. | Developer/team/CI | Debug config lặp lại sau pull/clone/switch branch. | Có vẻ Rule/Docker/Makefile có thể đủ, không nhất thiết cần AI. |
| 7 | An | Debug lỗi giữa frontend, backend và database mất thời gian vì phải kiểm tra nhiều layer. | Full-stack developer | Xác định root cause giữa request, response, backend log và database. | Workflow rõ, AI workflow có thể hỗ trợ, cần baseline thời gian/lỗi. |
| 8 | An | Khi nhận bug/feature, developer mất thời gian tìm đúng file/module cần sửa trong codebase lớn. | Developer | Search nhiều file và đọc dependency trước khi sửa. | Gần với coding agent use case, nhưng cần repo cụ thể để demo/validate. |
| 9 | An | Thành viên hỏi lại cách setup/chạy project vì tài liệu setup chưa dễ dùng. | Team member/developer | Setup knowledge nằm rải rác hoặc chưa chuẩn hóa. | Process/docs có thể giải quyết trước; AI chỉ cần nếu project phức tạp. |
| 10 | Quân | Task mới qua Messenger không có owner rõ, bị trôi và có thể bị quên. | Team lead và thành viên nhóm | Không có bước xác nhận owner và danh sách task chưa được nhận. | Rất mạnh cho group workflow; actor, bottleneck, metric đều rõ. |
| 11 | Quân | Thành viên hiểu sai task vì chi tiết nằm trong nhiều tin nhắn, dẫn đến rework. | Người implement và lead review | Không có task brief được xác nhận với goal, scope, workflow, acceptance criteria. | Pain thật, dễ validate với chat/task history, rất hợp bài toán nhóm. |
| 12 | Quân | Thành viên implement trùng scope vì owner/status/scope không nằm ở một source of truth. | Team lead và các dev | Thiếu liên kết giữa task, owner, branch/PR, status và deliverable. | Impact rõ nhưng có thể là biến thể của task ownership/source of truth. |
| 13 | Đạt | Business gửi ad-hoc data request mập mờ qua Slack, DA phải hỏi lại nhiều lần. | Fresher DA và stakeholder | Làm rõ time range, metric, filter, logic lọc qua nhiều tin nhắn. | Metric tốt, workflow rõ, AI workflow hợp, nhưng domain DA riêng hơn. |
| 14 | Đạt | Fresher DA mất 60-90 phút debug SQL dài kế thừa khi dashboard lệch số. | Fresher DA/senior DA | Đọc hiểu nhiều CTE/JOIN không có comment, phải bóc tách từng bước. | AI fit cao, metric tốt, nhưng cần query thật và data context để validate. |
| 15 | Đạt | Chuyển business request thành SQL draft mất 30-45 phút và dễ sai logic. | Fresher DA/business stakeholder | Dịch yêu cầu kinh doanh sang bảng, join, filter và SQL logic. | Có thể mạnh nếu nhóm chọn DA domain, rủi ro hallucinate schema. |
| 16 | Chương | Sinh viên và khách đến VinUni khó tìm phòng học/hội trường và quán ăn quanh Ocean Park vì thông tin vị trí bị phân tán. | Tân sinh viên, sinh viên trường khác, giảng viên thỉnh giảng, khách tham quan, sinh viên VinUni | Google Maps không đủ indoor map từng tầng; phải đi lòng vòng/hỏi bảo vệ hoặc tự lướt nhiều nguồn để tìm quán. | Nhóm chọn làm final vì actor rộng, pain dễ hiểu, có bối cảnh VinUni thật và có metric 15-20 phút/lần. |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A - Learning overload / knowledge retrieval | Duy #1, Duy #2 | Người học bị quá tải vì kiến thức và tài liệu nằm rải rác; khó biết phần nào đã hiểu/chưa hiểu hoặc tìm lại đúng nguồn. | Gần nhất với bối cảnh khóa AI hiện tại. Cần đo bằng quiz/checklist hoặc time log tìm tài liệu. |
| B - Team task coordination / source of truth | Duy #3, Quân #1, Quân #2, Quân #3 | Nhóm làm việc qua chat/GitHub nhưng task thiếu owner, scope, status, brief và deliverable chính thức. | Cluster mạnh nhất về teamwork; nhiều thành viên có pain tương tự. Có thể validate bằng task/chat history. |
| C - Developer workflow / debugging / code review | Quang #2, Quang #3, An #1, An #2, An #3 | Developer mất thời gian hiểu code, debug nhiều layer, setup môi trường hoặc review PR. | Hợp với coding agent, nhưng cần repo/test/log cụ thể để đo. |
| D - Data analyst request / SQL workflow | Đạt #1, Đạt #2, Đạt #3 | DA mất thời gian làm rõ request, đọc/debug SQL cũ và chuyển business logic thành SQL. | Metric khá rõ, AI fit tốt, nhưng domain hơi riêng so với cả nhóm nếu không ai khác làm DA. |
| E - Weekly reporting | Quang #1 | Từ nhiều nguồn raw data, người làm phải viết lại thành progress narrative. | Metric rõ, nhưng candidate này đứng một mình, ít trùng với các bài khác. |
| F - Campus navigation / student daily utility | Chương #1 | Người mới hoặc khách ở VinUni khó tìm đúng phòng/tầng/lối đi, rồi tiếp tục mất thời gian tìm tiện nghi/quán ăn quanh trường. | Bối cảnh rất local, dễ demo bằng VinUni/Ocean Park, actor rộng hơn một nhóm học. |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| A. Tìm phòng học/hội trường trong VinUni và tiện nghi/quán ăn quanh Ocean Park | Đây là final choice. Actor rộng: tân sinh viên, khách, giảng viên thỉnh giảng và sinh viên hiện tại đều có thể gặp. Workflow rất dễ hiểu: nhận mã phòng/nhu cầu ăn, tra map, hỏi đường/lướt app, rồi bị trễ hoặc mất thời gian. Có metric ban đầu 15-20 phút/lần và target dưới 2 phút. | Cần có dữ liệu indoor map đủ tin cậy và danh sách quán/giờ mở cửa không bị sai. Nếu scope gom cả phòng học và quán ăn thì có thể hơi rộng, cần ưu tiên "tìm phòng học trong VinUni" trước. |
| B. Sau ngày học/lab AI, sinh viên không biết phần nào đã hiểu và phần nào còn thiếu | Đây là second choice từ Duy. Rất sát bối cảnh lớp hiện tại; có actor rõ là sinh viên; workflow có lecture, lab, teamwork, VLearn, GitHub, presentation và feedback. Pain có con số ban đầu 40-60% kiến thức tự ước lượng. | Cần đo "hiểu" bằng cách nào cho công bằng; nếu chỉ là feeling thì metric yếu. Cần validate xem các bạn khác có pain giống Duy không. |
| C. Task nhóm qua chat/GitHub thiếu owner, scope, status và brief nên bị trôi, hiểu sai hoặc làm trùng | Nhiều ý cá nhân trùng nhau; actor rõ là team lead và thành viên; metric có thể đo bằng task chưa có owner sau 24h, số lần hỏi lại, số rework/overlap. So sánh Rule/Workflow/Agent khá rõ. | Có thể process fix/GitHub Issue template đã đủ. Cần quyết định có xử lý Messenger/chat không, vì có rủi ro privacy và context thiếu. |
| D. Developer mất thời gian debug/tìm file/review code trong project nhiều layer | Nhiều bạn dev gặp pattern tương tự; workflow có thể vẽ rõ; coding agent có thể hỗ trợ phân tích log/codebase. | Cần repo thật và logs/PR để validate. Nếu không có dữ liệu cụ thể, bài dễ thành demo chung chung. |
| E. Fresher DA xử lý request/SQL bị nghẽn vì stakeholder mập mờ hoặc SQL cũ khó hiểu | Metric của Đạt khá cụ thể; workflow DA rõ; AI workflow fit với parse request, SQL explanation, SQL draft. | Domain riêng của một thành viên, nhóm còn lại có thể khó defend nếu bị hỏi sâu về DA/BigQuery/business logic. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| A. Campus navigation trong VinUni và tiện nghi quanh trường | 5 | 5 | 4 | 5 | 5 | 5 | 5 | 34 |
| B. Learning overload sau ngày học/lab AI | 5 | 4 | 3 | 3 | 5 | 3 | 5 | 28 |
| C. Team task coordination thiếu owner/scope/status/brief | 5 | 5 | 4 | 4 | 5 | 5 | 5 | 33 |
| D. Developer debug/code navigation/code review | 5 | 4 | 3 | 4 | 4 | 4 | 4 | 28 |
| E. DA request/SQL workflow | 5 | 5 | 5 | 5 | 3 | 4 | 3 | 30 |

> Ghi chú: sau khi thêm idea của Chương, nhóm chọn candidate Campus navigation làm final. Candidate learning support của Duy là lựa chọn thứ 2 nếu muốn quay về bối cảnh khóa AI trực tiếp hơn.

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Final choice: Sinh viên và khách đến VinUni gặp khó khăn khi tìm phòng học/hội trường trong tòa nhà phức tạp và tìm quán ăn phù hợp quanh Ocean Park vì thông tin indoor map và tiện nghi xung quanh bị phân tán.

Second choice: Learning support của Duy - sau một ngày học/lab AI dày đặc, sinh viên không biết phần nào đã hiểu thật và phần nào còn thiếu.
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn bài của Chương vì problem này rất dễ hiểu với người nghe và có actor rộng: tân sinh viên, khách tham quan, giảng viên thỉnh giảng và sinh viên hiện tại. Workflow cũng rõ: nhận mã phòng hoặc nhu cầu ăn uống, tra Google Maps/app khác, không đủ thông tin indoor map hoặc giờ mở cửa thực tế, rồi phải hỏi người khác hoặc đi lòng vòng. Pain có impact nhìn thấy ngay: trễ giờ học, mất 20-30 phút nghỉ trưa và tạo cảm giác bối rối cho người mới. Bài này cũng dễ validate nhanh trong campus bằng interview/survey và dễ demo/pitch hơn các bài cần repo code, Slack thật hoặc SQL thật.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
Learning support của Duy là lựa chọn thứ 2 vì rất sát trải nghiệm khóa AI hiện tại và có pain thật về quá tải kiến thức. Tuy nhiên metric "đã hiểu 40-60%" cần được đo cẩn thận hơn bằng quiz/checklist, nếu không dễ bị xem là cảm tính.

Team task coordination có nhiều người gặp và score cao, nhưng có rủi ro là GitHub Issues/template/process fix đã giải quyết được phần lớn mà chưa cần AI. Developer debug/code navigation và DA request/SQL đều có AI fit tốt, nhưng cần dữ liệu thật như repo/log/SQL/schema để defend chắc hơn trong thời gian lab. Weekly reporting có metric rõ nhưng ít trùng với các thành viên khác.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Nhóm chốt tạm final theo hướng Campus navigation của Chương. Điểm cần thống nhất tiếp theo là scope: nên ưu tiên tìm phòng học/hội trường trong VinUni trước, còn quán ăn/tiện nghi quanh Ocean Park có thể là phần mở rộng. Duy learning support được giữ làm backup/second choice nếu nhóm muốn quay lại problem sát khóa AI hơn.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | | | | |
| Survey / poll | | | | |
| Log / ticket / review (nếu có) | | | | |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text

```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text

```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1 ...: __' - ai làm] → [2 ...: __'] → [3 ...: __'] → [4 ... bottleneck: __'] → ...
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |

**Bottleneck chính (2-3 câu):**

```text

```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 ...: __' - máy] → [2 AI ...: __'] → [3 ... review: __' - boundary] → [4 ... gửi]

Fallback: ...
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | | | |
| Số bước | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Risk mới | | | |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** | |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ:
- Tôi sửa gì:

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) — Vì sao:
- Độ phức tạp: [ ] Thấp (1-2 bước) / [ ] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao:

**Bài toán nhóm nằm ở ô nào:**

```text

```

**Vì sao (2-3 câu):**

```text

```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không?
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh?
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không?
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?
5. Có hạ được từ Agent → Workflow → Rule không?

**Mức chọn:**

```text
[Rule / Workflow / Agent]
```

**Vì sao chọn (3-4 câu):**

```text

```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text

```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** (làm / không làm) | |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | |

### 6.3. Final decision

| Câu hỏi                               | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
| ---------------------------------------| --------------------| ----------------------|
| Actor + workflow rõ chưa?             |                    |                      |
| Baseline + metric đo được chưa?       |                    |                      |
| Data/input đủ dùng chưa?              |                    |                      |
| AI sai, hậu quả chấp nhận được không? |                    |                      |
| Có người review/owner không?          |                    |                      |
| Có cách non-AI đơn giản hơn không?    |                    |                      |

**Decision:**

```text
[Go / Not Yet / No-Go]
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text

```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text

```

**Nếu Not Yet — cần validate gì trước:**

```text

```

**Nếu No-Go — làm gì thay AI:**

```text

```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text

```

---

### Self-check nộp phần 02 (nhóm)
- [ ] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [ ] Có validation (quote thật) + research (link kiểm được)
- [ ] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [ ] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [ ] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
