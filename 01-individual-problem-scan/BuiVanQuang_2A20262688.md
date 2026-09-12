# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Bùi Văn Quang
- Mã học viên: 2A202602688
- Vai trò / bối cảnh: Sinh viên năm cuối
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Viết báo cáo tiến độ
  - Review code của teammates
  - Chạy test tự động
  - Fix bug tìm được
  - Commit code + update docs

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Tốn thời gian | Mỗi tuần viết báo cáo tiến độ phải tìm dữ liệu từ nhiều nơi (Jira, local file, Slack, email) | Sinh viên, mentor, leader | **Mất ~60 phút/tuần** để gom dữ liệu + viết lại; hay bị trễ deadline thứ Hai |
| 2 | Lặp lại | Chạy test local phải lặp lại test suite → fail do config environment không đúng → phải tự debug | Sinh viên, CI/CD pipeline | **~10 phút × 3-4 lần/tuần**; hay phải xóa cache rồi chạy lại; config khác giữa máy các người |
| 3 | Pain từ người khác + AI có thể tốt hơn | Review code của teammates hay miss bug vì code khó hiểu, không có docstring rõ ràng | Reviewer (mình), teammates, team lead | **Review ~30 phút/lần** nhưng vẫn miss bug; phải hỏi lại ~2-3 câu/bản PR để hiểu intent |
| 4 | Tốn thời gian | Debug bug production mất lâu vì không biết bug ở đâu, phải đọc log dài, test lại nhiều lần | Sinh viên, end users (trực tiếp hoặc gián tiếp) | **~60 phút/bug** để tìm root cause; log không rõ ràng; không có stack trace đầy đủ |
| 5 | Lặp lại | Fix bug xong phải test lại nhiều lần vì fix sai hoặc regression mới | Sinh viên, team | **Fix 1 bug rồi test lại ~2-4 lần**; hay phải fix bug lặp lại trong sprint sau |
| 6 | Tốn thời gian | Commit code + update docs (README, API doc) lặp lại format → chậm, hay bị bỏ sót docs | Sinh viên, reviewer | **~15-20 phút/commit** để chuẩn bị docs; hay bị comment "docs không đúng" lặp lại |
| 7 | Lặp lại | Mỗi sprint mới lại phải setup environment dev lại (dependencies, config local, database setup) | Sinh viên | **Lần đầu ~1h30, lần sau ~30 phút**; hay bị lỗi vì có người chưa update docs setup; 5-6 lần/semester |
| 8 | Pain từ người khác | Teammates hỏi "làm sao fix cái bug này?" nhưng tôi phải tìm lại cách từng fix lần trước vì không ghi memo | Team, tôi | **~15-20 phút/lần hỏi lặp lại**; khoảng 2-3 lần/tháng bị hỏi cách fix lại vấn đề cũ |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Viết báo cáo tiến độ hằng tuần | Workflow rõ (6 bước), mất nhiều thời gian (60 phút/tuần), AI có thể draft từ dữ liệu sẵn có | Có cần ghi memo hay chỉ viết báo cáo thôi? Độ rõ ràng của báo cáo "đủ tốt" là bao nhiêu? |
| 2 | Review code của teammates khó vì code không có docstring, hay miss bug | Bottleneck rõ (hiểu code), impact cao (30 phút/lần + miss bug), AI có thể explain code logic + highlight potential bug | Reviewer sẵn sàng dùng AI hay sợ AI sai? Impact của miss bug bao lâu mới phát hiện? |
| 3 | Test chạy fail do config environment không đúng giữa máy các người | Lặp lại nhiều lần (10 phút × 3-4 lần/tuần), bottleneck rõ (config), Rule/Script có thể auto fix | Setup environment có script sẵn chưa? Config khác nhau chỉ do OS hay còn đó? |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Viết báo cáo tiến độ hằng tuần

```text
Problem 1 câu:
Mỗi tuần phải viết báo cáo tiến độ từ nhiều nguồn khác nhau (Jira, local file, Slack, email), mất khoảng 60 phút vì phải tìm dữ liệu, gom lại, và viết lại thành narrative mà mentor/leader hiểu được.

Actor:
Sinh viên (mình), Mentor, Team lead — người nhận báo cáo để tracking progress

Thời điểm / bối cảnh:
Hằng tuần (Friday hoặc Monday), trước buổi sync với mentor/leader

Current workflow 3-7 bước:
1. Đọc Jira board xem task đã làm tuần này (5 phút)
2. Lấy metrics từ local file/log (task count, bug fixed, test pass rate) (5 phút)
3. Đọc Slack recap hoặc email liên lạc từ mentor (10 phút)
4. Tổng hợp vào Google Docs hoặc Email draft (10 phút)
5. Viết narrative: summary tuần, achievement, bottleneck/risk, plan tuần sau (25 phút) <-- bottleneck
6. Self-review + format (3 phút)
7. Gửi email cho mentor/leader (2 phút)

Bottleneck:
Bước 5 — viết narrative từ raw data mất 25 phút vì phải tự ghép các thông tin từ nhiều nguồn, tự quyết định cái nào highlight, cái nào risk, cái nào là plan tiếp theo. Hay bị "blank page" syndrome.

Impact:
- **Mất ~60 phút/tuần** cho 1 người × 1 tuần = công sức lớn.
- Báo cáo hay trễ deadline → mentor/leader không có bối cảnh trước buổi sync.
- Nếu 5 sinh viên trong team mỗi người viết báo cáo riêng = 300 phút/tuần bị lãng phí vào viết lại dữ liệu thành narrative.

Success metric:
- Giảm thời gian từ 60 phút xuống dưới 20 phút/tuần.
- Không tăng số câu hỏi "sửa lại báo cáo" từ mentor/leader.
- Báo cáo phải gửi được trước 6pm Friday (không trễ).

Non-AI alternative:
- Template report cố định + Jira dashboard tự động pull metrics → giảm format effort nhưng chưa giải quyết tốt việc "viết narrative" tuần khác nhau, cách hiểu khác nhau.

AI hypothesis:
AI hỗ trợ cấu trúc dữ liệu từ nhiều nguồn + draft narrative từ dữ liệu đó. Sinh viên vẫn review + edit trước gửi.

Quick gut:
[x] Workflow (không phải No AI / Rule / Agent vì workflow là tuyến tính, AI chỉ hỗ trợ 1-2 bước ngôn ngữ, sinh viên vẫn review)
```

**Draft workflow Card #1** (ASCII):

```text
CURRENT STATE — 60 phút

[1 Đọc Jira: 5']
→ [2 Lấy metrics: 5']
→ [3 Đọc Slack: 10']
→ [4 Tổng hợp Docs: 10']
→ [5 Viết narrative: 25']  <-- bottleneck (khó)
→ [6 Review + format: 3']
→ [7 Gửi: 2']

FUTURE STATE — 18 phút

[1 Auto-pull Jira + metrics: 2']
→ [2 AI cấu trúc dữ liệu: 1']
→ [3 AI draft narrative từ template: 1']
→ [4 Sinh viên review + edit: 12']  <-- human boundary
→ [5 Gửi: 2']

Fallback: AI draft tệ/sai → sinh viên bỏ draft, tự viết lại từ đầu (quay về 25 phút original).

Bottleneck mới: Review + edit (12 phút) — đây là bottleneck chấp nhận được vì đó là điểm kiểm soát chất lượng.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Review code khó hiểu, hay miss bug

```text
Problem 1 câu:
Khi review PR của teammates, code không có docstring rõ ràng → phải đọc lâu để hiểu intent → hay miss bug → phải hỏi lại 2-3 câu/PR để clarify, rồi review lại.

Actor:
Reviewer (mình), Code author (teammates), Team lead (người merge PR)

Thời điểm / bối cảnh:
Mỗi khi có PR mới (2-3 lần/tuần), phải review trong vòng 24h để author không chờ quá lâu

Current workflow 3-7 bước:
1. Nhận thông báo PR mới trên GitHub (1 phút)
2. Đọc PR description + commit message để hiểu intent (3 phút)
3. Đọc code dòng-by-dòng để hiểu logic → khó vì không có comment/docstring (20 phút)  <-- bottleneck
4. Chỉ ra code issues/suggestions dạng comment (3 phút)
5. Author reply/fix (ngày hôm sau hoặc vài giờ sau)
6. Review lại code fixed (5 phút)
7. Approve + merge (2 phút)

Bottleneck:
Bước 3 — đọc code 20 phút (vừa lâu vừa dễ miss bug). Mặc dù code có syntax highlight nhưng không có high-level explanation của author, nên phải suy đoán intent từ code structure.

Impact:
- **~30 phút/lần review** (bước 1-4), và phải review lại 2-3 lần/PR.
- **Miss bug**: ~ 2-3 bug/sprint phát hiện bởi QA hoặc user sau khi merged, không phát hiện trong review.
- **Author phải hỏi lại**: "Cái chỗ này bạn review có hiểu không?", "Bạn có thấy logic sai ở chỗ này không?" → communication overhead.
- Nếu miss bug lại deploy production → phải fix hotfix → mất thêm vài giờ.

Success metric:
- Giảm thời gian review từ 30 phút xuống dưới 15 phút/lần review (lần đầu).
- Không giảm số bug phát hiện trong review (vẫn catch >= 80% bug trước khi merge).
- Giảm số lần hỏi lại từ 2-3 xuống còn 0-1 lần/PR.

Non-AI alternative:
- Code review guideline + bắt author viết docstring trước PR → cải thiện nhưng phụ thuộc vào discipline của author, mất 10 phút author viết docstring → chuyển công sức sang author.

AI hypothesis:
AI read code → generate high-level explanation (intent, data flow, potential issue) → reviewer dùng để hiểu nhanh + spot bug dễ hơn. Reviewer vẫn make final decision.

Quick gut:
[x] Workflow (AI hỗ trợ bước 3 bằng code explanation, reviewer vẫn review + decide)
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 30 phút/lần review

[1 Nhận PR: 1']
→ [2 Đọc description: 3']
→ [3 Đọc code line-by-line: 20']  <-- bottleneck (khó hiểu, miss bug)
→ [4 Comment issues: 3']
→ [5 Author fix (chờ)]
→ [6 Review lại: 5']
→ [7 Approve: 2']

Lặp lại 2-3 lần/PR = 60-90 phút tổng.

FUTURE STATE — 15 phút/lần review (lần đầu)

[1 Nhận PR: 1']
→ [2 Đọc description: 3']
→ [3 AI generate code explanation + potential bug alert: 2']
→ [4 Reviewer skim AI output + re-check code: 5']  <-- human boundary
→ [5 Comment + approve: 4']

Fallback: AI explanation sai/nhạt → reviewer ignore AI, tự đọc code như bình thường (quay về 20 phút).
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Test chạy fail do config environment không đúng

```text
Problem 1 câu:
Mỗi tuần phải chạy test local, nhưng test hay fail do config environment không giống nhau giữa máy các người (Python version, dependencies version, database config, env vars) → phải tự debug config rồi chạy lại test → 10 phút × 3-4 lần/tuần.

Actor:
Sinh viên (mình), CI/CD pipeline, Teammates (khi ngồi cùng debug), Tech lead (setup CI config)

Thời điểm / bối cảnh:
Sau khi pull code mới từ main branch, hoặc khi clone repo lần đầu, hoặc khi switch branch có dependency thay đổi

Current workflow 3-7 bước:
1. Pull code mới / clone repo (2 phút)
2. Chạy test local: `pytest` hoặc `npm test` (5 phút)
3. Test fail → xem error message → debug config (3 phút)
4. Thử fix: cài lại dependency, xóa cache, chuyển Python version (7 phút)  <-- bottleneck
5. Chạy test lại (5 phút)
6. Vẫn fail? Hỏi teammate hoặc tech lead (5 phút)
7. Cuối cùng test pass (2 phút)

Bottleneck:
Bước 4 — debug config mất 7 phút nhưng phải repeat 3-4 lần/tuần (vì mỗi lần pull hoặc branch switch lại phát sinh config issue khác nhau).

Impact:
- **~10 phút × 3-4 lần/tuần = 40 phút/tuần** lãng phí vào chỉnh config.
- Test fail lâu → delay feedback về code quality → có bug syntax không biết.
- Nếu multi-OS team (Mac + Linux + Windows) → mỗi OS có config issue khác → communication overhead.
- Nếu team có 5 người mỗi người gặp vấn đề = 200 phút/tuần bị lãng phí.

Success metric:
- Giảm thời gian debug config từ 7 phút xuống dưới 2 phút (chỉ cần chạy 1 command).
- Test lần đầu pass rate >= 95% (chỉ fail nếu thật sự code sai, không phải config).
- Sau khi pull/clone, test chạy ngay được (không phải chỉnh gì thêm).

Non-AI alternative:
- **Rule/Script**: viết setup script tự động (setup.sh hoặc Makefile) → clone, chạy script, test chạy ngay. Đây là "No AI" solution nhưng hiệu quả.
- Docker container cho dev → test chạy trong container → config được đồng nhất.

AI hypothesis:
AI detect config issue từ error log → suggest fix command (install dependencies, set env vars, etc.) hoặc auto-run fix. Sinh viên vẫn review trước approve.

Quick gut:
[ ] No AI / process fix — **Rule/Script (setup script / Makefile / Docker) đủ rồi**, không cần AI. Có thể thêm AI để detect + suggest fix nếu script chưa cover hết scenario.
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 40 phút/tuần (= 10 phút × 4 lần)

[1 Pull code / clone: 2']
→ [2 Chạy test: 5']
→ [3 Test fail → xem error: 3']
→ [4 Debug config (fix deps, version, env vars): 7']  <-- bottleneck
→ [5 Chạy test lại: 5']
→ (Lặp lại bước 4-5 nếu vẫn fail)

Toàn bộ workflow cứ 2-3 ngày lặp lại 1 lần.

FUTURE STATE — 5 phút/lần (Rule/Script)

[1 Pull code / clone: 2']
→ [2 Chạy setup script (hoặc make setup): 1']  <-- tự động fix config
→ [3 Chạy test: 2']
→ Test pass (không phải debug)

Fallback: Script miss case mới → sinh viên debug như cũ (quay về 7 phút).

Alternative: Docker dev container → test chạy trong container → config được đồng nhất.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Viết báo cáo tiến độ — Problem Card #1
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Hằng tuần phải viết báo cáo tiến độ từ 4 nguồn khác nhau (Jira, local file, Slack, email) mất 60 phút.
Bottleneck là bước "viết narrative" (25 phút) vì phải tự ghép thông tin thành insight.
Impact là ~40 phút/tuần bị lãng phí (sau khi AI help), × 5 sinh viên trong team = 200 phút/tuần team có thể tiết kiệm.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Nếu AI draft báo cáo bằng thông tin từ Jira + local metrics, nhưng miss cái context từ Slack about bug lớn được phát hiện cuối tuần, thì AI sẽ làm gì? Có cách nào để AI "biết" nên include cái context đó không?

2. Báo cáo "đủ tốt" để mentor/leader hiểu và không phải hỏi lại có nghĩa là gì cụ thể? Là dùng từ chuyên môn rõ? Là format cố định? Là cần insight thực sự hay chỉ list facts đủ rồi?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
