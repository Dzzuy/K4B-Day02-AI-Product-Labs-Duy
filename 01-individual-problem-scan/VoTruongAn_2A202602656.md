# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:Võ Trường An
- Mã học viên:2A202602656
- Vai trò / bối cảnh: Sinh viên IT năm cuối, làm Full Stack Developer/AI Developer trong các project cá nhân và nhóm.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
Phát triển frontend bằng React/Next.js và backend bằng FastAPI.
Làm các tính năng AI/data bằng Python.
Debug và sửa lỗi giữa frontend, backend, database.
Làm việc nhóm, quản lý code qua Git/GitHub.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Tốn thời gian | Khi làm feature mới, phải đọc nhiều file/code để hiểu luồng frontend → backend → database trước khi sửa | Developer | Mỗi lần debug feature thường phải mở nhiều file; **[CẦN ĐO 3 lần]** |
| 2 | Lặp lại | Sau khi sửa backend API phải kiểm tra lại API bằng Postman rồi mới nối frontend | Developer | Xảy ra nhiều lần trong mỗi feature; **[Đếm số API test/tuần]** |
| 3 | Tốn thời gian | Debug lỗi frontend/backend phải lần lượt kiểm tra request, response, log backend và database | Developer | Một lỗi thường qua nhiều bước kiểm tra; **[CẦN ĐO thời gian trung bình/lỗi]** |
| 4 | Lặp lại | Viết và cập nhật tài liệu API khi endpoint thay đổi | Developer/team member | Endpoint thay đổi thì documentation phải cập nhật lại; **[Đếm số endpoint thay đổi/tuần]** |
| 5 | Pain từ người khác | Thành viên trong nhóm hỏi lại cách chạy project hoặc cách cấu hình môi trường | Team member | Các câu hỏi thường xoay quanh setup, environment và command chạy project; **[Đếm số lần hỏi/tuần]** |
| 6 | Pain từ người khác | Khi merge code, thành viên phải xử lý conflict hoặc hỏi nhau về phần code đã thay đổi | Developer/team | Xảy ra khi nhiều người sửa cùng khu vực; **[Đếm số conflict/tuần]** |
| 7 | AI có thể tốt hơn | Khi đọc một thư viện/API mới, phải tự lọc documentation để tìm đúng phần cần dùng | Developer | Mỗi lần tích hợp công nghệ mới đều phải tìm docs/examples; **[CẦN ĐO thời gian tìm 3 lần]** |
| 8 | Tốn thời gian | Khi AI sinh code, phải đọc lại và kiểm tra xem code có đúng với architecture hiện tại không | Developer | AI có thể tạo code nhanh nhưng cần review thủ công; **[Đếm số lần phải sửa AI-generated code]** |
| 9 | Lặp lại | Khi hoàn thành feature phải tự kiểm tra nhiều trường hợp trước khi commit/push | Developer | Mỗi feature đều có bước test thủ công; **[Đếm số test/checklist mỗi feature]** |
| 10 | AI có thể tốt hơn | Khi project có nhiều module, khó tìm nhanh nơi cần sửa khi một feature bị lỗi | Developer | Phải search qua nhiều file/module; **[CẦN ĐO thời gian tìm file liên quan]** |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:“Tôi là sinh viên IT năm cuối, thường làm Full Stack với React/Next.js, FastAPI và Python cho AI/data, đồng thời làm project nhóm qua GitHub. Hãy gợi ý thêm các problem theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn, pain từ người khác. Với mỗi problem, xác định actor, workflow và cách đo. Không đưa ý tưởng quá rộng.”
- Ý dùng được:Các problem liên quan đến debug, tìm hiểu codebase, API/documentation, team setup và review code.
- Ý bỏ vì không phải pain thật:Các ý kiểu “AI tự quản lý toàn bộ project”, “AI tự code toàn bộ ứng dụng”, “AI thay thế developer” vì quá rộng và chưa xác định được workflow/bottleneck cụ thể.

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
| 1 | Debug lỗi giữa Frontend → Backend → Database | Workflow rõ; xảy ra trong quá trình dev; có thể đo thời gian/lỗi | Cần đo baseline trung bình |
| 2 | Tìm hiểu codebase để xác định nơi cần sửa | Có pain rõ khi project lớn; có thể dùng AI hỗ trợ code navigation | Cần xác định chính xác thời gian mất cho mỗi issue |
| 3 | Team member hỏi lại cách setup/chạy project | Actor rõ; workflow lặp lại; có thể giải bằng documentation trước khi cần AI | Cần đếm số lần hỏi/tuần |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Tên problem]

```text
Problem 1 câu:Khi một feature bị lỗi, developer phải lần lượt kiểm tra ƒfrontend request,
backend API, log và database để xác định nguyên nhân, khiến thời gian debug
tăng lên và workflow bị gián đoạn.

Actor:Developer đang phát triển và debug ứng dụng Full Stack.

Thời điểm / bối cảnh:Trong quá trình phát triển feature hoặc sau khi tích hợp frontend,
backend và database.

Current workflow 3-7 bước:
1. Nhận thấy feature/API hoạt động sai
2. Kiểm tra request từ frontend
3. Kiểm tra response/status code
4. Kiểm tra log backend
5. Kiểm tra database/data liên quan
6. Xác định nguyên nhân và sửa code
7. Chạy lại để kiểm tra

Bottleneck:Xác định nguyên nhân giữa nhiều layer frontend/backend/database.

Impact:Developer mất thời gian chuyển qua nhiều layer để tìm nguyên nhân;
việc debug làm gián đoạn tiến độ phát triển feature.

Success metric:Giảm thời gian trung bình để xác định root cause của một lỗi.
Baseline cần đo trên ít nhất 3 lỗi thực tế.

Non-AI alternative:Chuẩn hóa logging, error message, API contract và debugging checklist.

AI hypothesis:AI phân tích error message, request/response và log để gợi ý
layer/nguyên nhân có khả năng gây lỗi, sau đó developer tự kiểm tra.


Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — [CẦN ĐO]

[Frontend lỗi]
	↓
[Kiểm tra request]
	↓
[Kiểm tra response]
	↓
[Kiểm tra backend log]  <-- bottleneck
	↓
[Kiểm tra database]
	↓
[Tìm root cause]
	↓
[Sửa + test lại]

FUTURE STATE — [CẦN ĐO]

[Thu thập error/request/log]
	↓
[AI phân tích + gợi ý root cause]
	↓
[Developer verify]
	↓
[Sửa + test lại]

Human boundary:
Developer phải xác nhận nguyên nhân trước khi sửa code.

Fallback:
Nếu AI phân tích sai hoặc không đủ context → developer quay về
debugging checklist thủ công.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu:

Khi một feature hoặc bug liên quan đến nhiều module, developer phải
tìm kiếm thủ công qua nhiều file để xác định component, API hoặc service
cần thay đổi.

Actor:

Developer làm việc trên project Full Stack.

Thời điểm / bối cảnh:

Khi nhận bug/feature mới trong codebase có nhiều module.

Current workflow:

1. Đọc yêu cầu/bug
2. Search keyword trong codebase
3. Mở các file liên quan
4. Đọc luồng component/API/service
5. Xác định file cần sửa
6. Thay đổi code
7. Test lại

Bottleneck:

Xác định đúng các file/module liên quan trước khi bắt đầu sửa.

Impact:

Mất thời gian đọc code và có nguy cơ sửa sai vị trí hoặc bỏ sót dependency.

Success metric:

Giảm thời gian từ lúc nhận issue đến lúc xác định được các file/module
cần thay đổi.

Non-AI alternative:

Chuẩn hóa architecture, naming convention, folder structure và documentation.

AI hypothesis:

AI phân tích issue + codebase để gợi ý các file/module liên quan
và giải thích dependency giữa chúng.

Quick gut:

[ ] No AI / process fix

[ ] Rule

[x] Workflow

[ ] Agent

[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — [CẦN ĐO]

[Đọc issue]
   →
[Search keyword]
   →
[Mở nhiều file]
   →
[Đọc dependency]
   →
[Xác định nơi sửa]  <-- bottleneck
   →
[Code]
   →
[Test]

FUTURE STATE — [CẦN ĐO]

[Đọc issue]
   →
[AI phân tích codebase]
   →
[AI đề xuất file/module liên quan]
   →
[Developer verify]  <-- human boundary
   →
[Code]
   →
[Test]

Fallback:
Nếu AI đề xuất sai → developer sử dụng search + architecture/documentation
như workflow hiện tại.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu:

Khi thành viên mới hoặc thành viên khác quay lại project, họ thường phải
hỏi lại cách setup environment và chạy project thay vì tự tìm được câu trả lời.

Actor:

Thành viên trong nhóm phát triển phần mềm.

Thời điểm / bối cảnh:

Khi clone project trên máy mới, pull thay đổi lớn hoặc setup lại environment.

Current workflow:

1. Clone/pull repository
2. Đọc README
3. Cài dependency
4. Cấu hình environment
5. Chạy project
6. Gặp lỗi
7. Hỏi thành viên khác

Bottleneck:

Khi documentation không đủ rõ hoặc không cập nhật theo codebase.

Impact:

Người gặp lỗi phải chờ người khác hỗ trợ; người có kinh nghiệm bị gián đoạn
để trả lời các câu hỏi setup lặp lại.

Success metric:

Giảm số câu hỏi setup lặp lại trong nhóm và giảm thời gian từ clone
đến khi chạy project thành công.

Non-AI alternative:

README chuẩn hóa + setup script + .env.example + troubleshooting checklist.

AI hypothesis:

AI đọc README, cấu trúc project và error message để hướng dẫn thành viên
từng bước xử lý lỗi setup.

Quick gut:

[ ] No AI / process fix

[x] Rule

[x] Workflow

[ ] Agent

[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — [CẦN ĐO]

[Clone repo]
    →
[Đọc README]
    →
[Cài dependency]
    →
[Setup .env]
    →
[Run project]
    →
[Gặp lỗi]
    →
[Hỏi teammate]  <-- bottleneck

FUTURE STATE — [CẦN ĐO]

[Clone repo]
    →
[README + setup script]
    →
[Run project]
    →
[Nếu lỗi → AI hướng dẫn]
    →
[Developer verify]  <-- human boundary
    →
[Project chạy]

Fallback:
Nếu AI không giải quyết được → gửi error cho teammate/maintainer.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Card tôi muốn pitch nhất: Debug lỗi giữa Frontend → Backend → Database.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Tôi chọn bài này vì đây là workflow xảy ra trực tiếp trong quá trình phát triển Full Stack và có các bước khá rõ từ lúc phát hiện lỗi đến khi tìm được root cause. Bottleneck nằm ở việc phải chuyển qua nhiều layer để kiểm tra request, response, backend log và database. Nếu đo được thời gian debug trên một số lỗi thực tế, nhóm có thể so sánh rõ before/after và đánh giá AI có thực sự giúp giảm effort hay không.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Nếu chuẩn hóa logging, error message và debugging checklist đã giải quyết được phần lớn vấn đề, liệu có thực sự cần AI không?

Nếu dùng AI, AI nên chỉ gợi ý root cause hay có nên cho AI tự đề xuất code sửa lỗi?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
