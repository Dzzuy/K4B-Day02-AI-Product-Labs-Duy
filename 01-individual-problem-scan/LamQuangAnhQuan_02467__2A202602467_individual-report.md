# 01 — Individual Problem Scan

> Thực hiện theo Phase 1 và Phase 2 trong 01-worksheet.md. Nội dung dựa trên trải nghiệm thật khi tôi lead nhóm 4 thành viên. Những baseline chưa có log được ghi rõ là chưa đo, không tự tạo số liệu.

## Thông tin cá nhân

- Họ và tên: Lâm Quang Anh Quângit
- Mã học viên: 2A202602467
- Vai trò / bối cảnh: Sinh viên, team lead của nhóm 4 thành viên phát triển và liên tục cải tiến một sản phẩm phần mềm.
- Công việc hằng tuần:
  - Sử dụng sản phẩm để phát hiện bug hoặc nhu cầu chức năng mới.
  - Xác định scope và giao task qua Messenger/GitHub.
  - Theo dõi owner, tiến độ và các task chưa được nhận.
  - Review kết quả, phản hồi và cùng nhóm chọn solution.
  - Kiểm tra code, tài liệu và deliverable trước khi tích hợp.

---

## Phase 1 — Scan 5+ problems

### Bối cảnh scan

Messenger là nơi trao đổi chính; task và code xuất hiện trên cả Messenger và GitHub. Ghép nhóm random hoặc ghép nhóm với người lạ (các thành viên không quên biết nhau, không hiễu rõ về năng lực cá nhân của nhau). Nhóm làm theo hướng Agile: dùng sản phẩm, phát hiện vấn đề rồi giao việc và cải tiến liên tục. Bằng chứng ban đầu là quan sát trực tiếp của tôi với vai trò lead; tần suất và thời gian cần được ghi log thêm.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Pain từ người khác | Lead đăng task trên Messenger nhưng thành viên thường không chủ động xác nhận nhận việc. | Lead và 3 thành viên | Nhóm 4 người; theo quan sát của lead, hầu hết thành viên đợi được chỉ định. Tỷ lệ chính xác chưa có log. |
| 2 | Lặp lại | Task chưa có người nhận bị trôi khi nhóm thảo luận việc khác và có thể bị quên. | Cả nhóm | Nếu lead không chỉ định hoặc nhắc lại thì task có thể không được thực hiện. Số task/sprint chưa thống kê. |
| 3 | Tốn thời gian | Lead phải quay lại Messenger, tìm task chưa có owner rồi chỉ định thủ công. | Team lead | 1 lead điều phối 3 thành viên; việc theo dõi hiện dựa vào trí nhớ và lịch sử chat. Thời gian/tuần chưa đo. |
| 4 | Lặp lại | Thành viên quên nội dung lead đã nhắn khi thông tin bị đẩy lên bởi thảo luận mới. | Thành viên và lead | Cả 4 thành viên dùng Messenger; đã có trường hợp lead phải nhắc lại. |
| 5 | Tốn thời gian | Chi tiết task nằm trong nhiều tin nhắn nên thành viên phải tự ghép mục tiêu, scope và workflow. | Thành viên nhận task | Có 2 nguồn công việc là Messenger và GitHub; chưa có task brief thống nhất. |
| 6 | Pain từ người khác | Thành viên quên hoặc hiểu sai chi tiết task, dẫn đến sai workflow và sai kết quả. | Người implement và lead review | Lỗi đã được lead quan sát; số lần và thời gian rework chưa thống kê. |
| 7 | Tốn thời gian | Lead phải giải thích và review lại khi kết quả không đúng workflow hoặc scope. | Lead và thành viên | Mỗi trường hợp ảnh hưởng ít nhất 2 người; thời gian rework chưa đo. |
| 8 | Tốn thời gian | Kết quả được gửi phân tán giữa Messenger và GitHub nên khó xác định bản chính thức. | Lead và cả nhóm | Có ít nhất 2 nơi nhận kết quả; chưa có quy ước duy nhất cho mọi deliverable. |
| 9 | Lặp lại | Feedback nằm trong các đoạn chat khác nhau nên có thể bị quên hoặc được nhắc lại trùng nhau. | Người nhận feedback và người review | Nhóm có 4 người cùng trao đổi; số feedback bỏ sót/trùng chưa được đếm. |
| 10 | Pain từ người khác | Thành viên implement trùng scope vì không thấy rõ ai đang làm gì và ranh giới task. | Thành viên và lead | Đã có trường hợp implementation trùng scope; số giờ lãng phí chưa thống kê. |

### Baseline cần thu thập

Trong 2 tuần tiếp theo, tôi sẽ ghi tổng số task, số task chưa có owner sau 24 giờ, thời gian từ giao đến nhận, số task bị quên, số task rework do hiểu sai, số lần trùng scope, thời gian tìm deliverable và số feedback bị bỏ sót/trùng.

### AI đã dùng ở Phase 1

- Prompt đã hỏi: Gợi ý problem từ trải nghiệm lead nhóm với task không ai nhận, tin nhắn bị trôi, hiểu sai yêu cầu, kết quả phân tán, feedback bị quên/trùng và implementation trùng scope.
- Ý dùng được: Gom pain thành task ownership, task understanding, result management, feedback và decision.
- Ý bỏ: Các problem riêng về dependency, SSD và notebook vì không cùng bối cảnh làm việc nhóm.

### Self-check Phase 1

- [x] Có 10 problem và actor cụ thể.
- [x] Dùng ít nhất 3 lăng kính.
- [x] Bắt đầu từ problem, không bắt đầu từ bot.
- [ ] Baseline định lượng cần được ghi log hoặc validation thêm.

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Task không có người nhận bị trôi và bị quên | Actor, workflow và hậu quả rõ; đo được bằng thời gian có owner và số task bị quên; so sánh được Rule/Workflow/Agent. | Chưa có số task/sprint và tỷ lệ chưa có owner sau 24 giờ; chưa biết process fix đã đủ hay cần bot. |
| 2 | Thành viên hiểu sai task, dẫn đến sai workflow và sai kết quả | Đã có quan sát thật; ảnh hưởng cả người làm và lead; đo được bằng số lần và thời gian rework. | Chưa tách được lỗi do tin nhắn bị trôi với lỗi do task ban đầu chưa rõ. |
| 3 | Thành viên implement trùng scope | Lãng phí công của nhiều người; liên quan trực tiếp đến Messenger/GitHub; đo được số overlap và thời gian bị bỏ. | Chưa rõ nguyên nhân chính là thiếu task board, scope mơ hồ hay không cập nhật trạng thái. |

---

#### Problem Card #1 — Task không có owner và bị quên

**Problem 1 câu:**
Trong nhóm phát triển sản phẩm gồm 4 thành viên, task mới được giao qua Messenger nhưng thành viên thường chờ lead chỉ định thay vì xác nhận nhận việc; nếu lead không tiếp tục theo dõi, task có thể bị trôi và bị quên.

**Actor:** Team lead điều phối và 3 thành viên nhận task.

**Bối cảnh:** Khi nhóm phát hiện bug hoặc nhu cầu chức năng mới trong chu kỳ cải tiến Agile.

**Current workflow:**

1. Nhóm phát hiện bug/chức năng mới.
2. Lead mô tả task trên Messenger.
3. Lead chờ thành viên chủ động nhận.
4. Nhóm chuyển sang thảo luận việc khác.
5. Lead phải nhớ để quay lại chỉ định; nếu không, task bị quên.
6. Thành viên được chỉ định mới bắt đầu làm.

**Bottleneck:** Bước 3–5: không có bước xác nhận owner và không có danh sách task chưa được nhận.

**Impact:** Task có thể không được thực hiện; lead phải nhớ trạng thái bằng lịch sử chat; tiến độ phụ thuộc vào việc lead có nhớ để nhắc.

**Success metric:**

- Đo baseline: tổng task, số task chưa có owner sau 24 giờ và thời gian trung vị từ lúc giao đến lúc nhận.
- Pilot: 100% task có trạng thái và owner xác nhận trong 24 giờ.
- Không còn task bị quên vì chưa có owner.
- Không tăng thời gian quản lý thủ công của lead.

**Non-AI alternative:** Template giao task và GitHub Issues/Projects; mỗi task bắt buộc có owner, scope, deadline, acceptance criteria và trạng thái.

**AI hypothesis:** Bot đọc phần thảo luận được cho phép, phát hiện task, tạo task nháp, cảnh báo task chưa có owner và đề xuất người phù hợp từ kỹ năng đã khai báo cùng workload. Lead duyệt trước khi tạo hoặc giao task chính thức.

**Quick gut:** Workflow có AI. Tầm nhìn dài hạn có thể là Agent, nhưng pilot phải có lead xác nhận.

**Draft workflow:**

    CURRENT STATE — baseline chưa đo
    [Phát hiện việc] → [Lead nhắn task] → [Chờ tự nhận] <-- bottleneck
    → [Tin nhắn trôi] → [Lead chỉ định / Task bị quên] → [Thực hiện]

    FUTURE STATE — owner xác nhận trong 24 giờ
    [Thảo luận] → [Bot tạo task nháp] → [Lead duyệt] <-- human boundary
    → [Lưu task chính thức] → [Thành viên nhận] → [Nhắc task unassigned]

    Fallback: bot trích xuất sai thì lead sửa hoặc bỏ bản nháp.
    Bot không tự giao task khi lead chưa duyệt.

---

#### Problem Card #2 — Thành viên hiểu sai chi tiết task

**Problem 1 câu:**
Chi tiết task được trao đổi qua nhiều tin nhắn Messenger nên thành viên có thể quên hoặc hiểu thiếu mục tiêu, workflow và scope, dẫn đến implementation sai và phải rework.

**Actor:** Thành viên nhận task và team lead review.

**Bối cảnh:** Sau khi giao sửa bug hoặc phát triển chức năng và trước khi implement.

**Current workflow:**

1. Lead nhắn yêu cầu ban đầu.
2. Nhóm bổ sung chi tiết qua nhiều tin nhắn.
3. Thành viên tự tìm và ghép thông tin.
4. Thành viên implement theo cách hiểu.
5. Lead phát hiện sai workflow/scope/output.
6. Lead giải thích lại và thành viên rework.

**Bottleneck:** Không có một task brief được xác nhận chứa goal, scope, workflow, acceptance criteria và quyết định mới nhất.

**Impact:** Lead và người implement mất thêm thời gian giải thích, sửa và review lại; kết quả có thể sai dù code đã hoàn thành.

**Success metric:**

- Đo baseline: số task rework do hiểu sai và tổng thời gian rework.
- Pilot: 100% task có task brief được thành viên xác nhận trước khi code.
- Giảm ít nhất 50% task rework do hiểu sai so với baseline.
- Câu trả lời của bot về yêu cầu phải có nguồn.

**Non-AI alternative:** Template task brief gồm problem, goal, in-scope, out-of-scope, workflow, deliverable và acceptance criteria; thành viên restate để lead xác nhận.

**AI hypothesis:** AI tổng hợp thảo luận thành task brief, theo dõi thay đổi và trả lời về task có dẫn nguồn. Lead duyệt; AI không tự thêm requirement hoặc biến ý kiến thành quyết định.

**Quick gut:** Workflow có AI.

**Draft workflow:**

    CURRENT STATE — baseline chưa đo
    [Lead nhắn] → [Thảo luận phân tán] → [Tự ghép thông tin] <-- bottleneck
    → [Implement] → [Phát hiện sai] → [Giải thích lại + rework]

    FUTURE STATE — giảm ít nhất 50% rework do hiểu sai
    [Thảo luận] → [AI tạo brief có nguồn] → [Lead duyệt] <-- human boundary
    → [Thành viên xác nhận] → [Implement] → [Review theo criteria]

    Fallback: AI sai hoặc thiếu thì lead chỉnh brief; thành viên xem lại nguồn
    và hỏi trực tiếp trước khi implement.

---

#### Problem Card #3 — Implementation trùng scope

**Problem 1 câu:**
Thông tin owner, trạng thái và ranh giới task không được cập nhật thống nhất giữa Messenger và GitHub, khiến thành viên có thể implement trùng scope và tạo solution dư thừa.

**Actor:** Các thành viên implement và team lead phân chia/review scope.

**Bối cảnh:** Khi nhiều bug hoặc chức năng được phát triển song song.

**Current workflow:**

1. Nhóm thảo luận nhiều vấn đề/solution trên Messenger.
2. Thành viên bắt đầu thực hiện.
3. Owner, trạng thái và scope không được cập nhật ở một nơi chung.
4. Thành viên khác làm một implementation có scope tương tự.
5. Lead phát hiện overlap khi review.
6. Nhóm phải chọn, ghép hoặc bỏ một phần kết quả.

**Bottleneck:** Thiếu một source of truth liên kết task, owner, scope, branch/PR, trạng thái và deliverable.

**Impact:** Lãng phí thời gian implement/review, có thể phát sinh merge conflict và công sức của một thành viên không được sử dụng.

**Success metric:**

- Đo baseline: số implementation overlap và số giờ cho phần trùng.
- Pilot: 100% task đang làm có owner, scope và link branch/PR.
- Không có overlap ngoài chủ ý trong thời gian pilot.
- Đo và giảm thời gian lead tìm owner/kết quả chính thức.

**Non-AI alternative:** Dùng GitHub Issues/Projects làm source of truth; mọi branch/PR liên kết issue; thành viên xác nhận scope trước khi code.

**AI hypothesis:** AI so sánh task, branch và PR đang mở để cảnh báo scope tương tự, tóm tắt điểm giống/khác giữa solution. Lead quyết định overlap có chủ ý hay cần tách.

**Quick gut:** Rule/process fix có thể đã đủ; chỉ thêm AI nếu so sánh scope bằng tay vẫn là bottleneck.

**Draft workflow:**

    CURRENT STATE — baseline chưa đo
    [Thảo luận] → [Bắt đầu code] → [Scope không cập nhật chung] <-- bottleneck
    → [Implementation overlap] → [Lead phát hiện] → [Bỏ/ghép/viết lại]

    FUTURE STATE — 0 overlap ngoài chủ ý trong pilot
    [Issue có scope] → [Gán owner + branch] → [Xác nhận trước khi code]
    → [Rule kiểm tra PR có issue] → [Cảnh báo tương tự]
    → [Lead xác nhận] <-- human boundary → [Implement và review]

    Fallback: cảnh báo sai thì lead bỏ cảnh báo và giữ hai task.
    GitHub Issue vẫn là nguồn chính thức.

---

### 2.3. Card muốn pitch nhất

**Card tôi muốn pitch nhất:** Problem Card #1 — Task không có owner và bị quên.

**Vì sao:**
Nhóm 4 người cải tiến sản phẩm liên tục nên bug và nhu cầu mới xuất hiện thường xuyên. Task được giao qua Messenger nhưng hầu hết thành viên chờ lead chỉ định; nếu lead không nhớ để quay lại, task có thể bị trôi và bị quên. Tôi muốn đo tỷ lệ task chưa có owner sau 24 giờ và thử workflow bảo đảm mọi task có owner, scope và trạng thái rõ.

**Câu hỏi tôi muốn nhóm challenge:**

1. Pain này có cần AI đọc và ghi nhớ tin nhắn, hay chỉ cần quy định mọi task phải là GitHub Issue có owner?
2. Bot nên được phép đề xuất hoặc giao task đến mức nào để không sai phân quyền và không đánh giá chủ quan năng lực thành viên?

**AI phản biện Card:**

- Điểm yếu AI chỉ ra: Ý tưởng ban đầu “bot hiểu mọi thứ và trả lời mọi câu hỏi” quá rộng, solution-first, chưa có baseline và có rủi ro quyền riêng tư, suy luận sai năng lực, task/decision giả.
- Tôi sửa gì: Thu hẹp pilot vào phát hiện task, tạo task nháp, theo dõi owner và trả lời câu hỏi điều phối có nguồn. Lead duyệt task, assignment và decision; kỹ năng thành viên do nhóm khai báo.

### Self-check nộp phần 01

- [x] Có 10 problems và top 3 Problem Cards.
- [x] Mỗi card có workflow trước/sau, bottleneck, metric dự kiến và fallback.
- [x] Đã chọn card pitch và câu hỏi challenge.
- [x] Đã phân biệt problem với ý tưởng bot/Agent.
- [ ] Baseline định lượng chưa hoàn tất; cần log hoặc validation với 3 thành viên trước khi coi target là kết quả đã kiểm chứng.
