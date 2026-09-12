# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên          | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
| -----| --------------------| -------------| ------------------------------------------------------------------|
| 1   | Phạm Đình Duy      | 2A202602913 | Synthesis, problem framing, learning pain                        |
| 2   | Bùi Văn Quang      | 2A202602688 | Developer workflow, reporting/code review/test pain              |
| 3   | Võ Trường An       | 2A202602656 | Full-stack debug, codebase navigation, setup pain                |
| 4   | Lâm Quang Anh Quân | 2A202602467 | Team coordination, task ownership, task clarity                  |
| 5   | Phạm Quốc Đạt      | 2A202602384 | Data analyst workflow, stakeholder request, SQL pain             |
| 6   | Nguyễn Hữu Chương  | 2A202602601 | Campus navigation, student/guest daily pain                      |

**Candidate problem nhóm chọn (1 câu):**

```text
Sinh viên và khách, giảng viên đến VinUni gặp khó khăn khi tìm phòng học/hội trường trong tòa nhà phức tạp và tìm quán ăn khu vực quanh VinUni
```
---

## Phase 3 — Group Convergence: từ candidates cá nhân về shortlist

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| #   | Người đưa ra | Candidate problem                                                                                                       | Người gặp vấn đề                                                                                | Điểm nghẽn                                                                                                    | Cảm nhận nhanh của nhóm                                                                               |
| -----| --------------| -------------------------------------------------------------------------------------------------------------------------| -------------------------------------------------------------------------------------------------| ---------------------------------------------------------------------------------------------------------------| -------------------------------------------------------------------------------------------------------|
| 1   | Duy          | Sau một ngày học AI dày đặc, sinh viên không biết phần nào đã hiểu thật và phần nào còn thiếu.                          | Sinh viên học lecture/lab AI                                                                    | Kiến thức nằm rải ở lecture, lab, VLearn, GitHub, presentation và feedback; chưa có self-check rõ.            | Rất gần bối cảnh lab hiện tại, pain thật, nhưng cần cách đo "đã hiểu" rõ hơn.                         |
| 2   | Duy          | Tìm lại tài liệu, yêu cầu hoặc đoạn hướng dẫn giữa VLearn, GitHub và link lớp mất lâu.                                  | Sinh viên/nhóm lab                                                                              | Nguồn phân tán, không có một index nguồn chuẩn.                                                               | Rõ workflow, dễ validate, có thể chỉ cần process/index trước khi AI.                                  |
| 3   | Duy          | Nhóm lab mất thời gian vì phân công, đầu ra và trạng thái task chưa rõ.                                                 | Nhóm lab                                                                                        | Task thiếu owner, output, deadline nhỏ và dependency.                                                         | Trùng pattern với idea của Quân, có khả năng gom thành cluster teamwork.                              |
| 4   | Quang        | Viết báo cáo tiến độ hằng tuần từ Jira, local file, Slack, email mất khoảng 60 phút.                                    | Sinh viên/mentor/team lead                                                                      | Viết narrative từ raw data, phải chọn highlight/risk/plan thủ công.                                           | Metric mạnh, workflow rõ, nhưng domain hơi lệch khỏi bài học/lab của cả nhóm.                         |
| 5   | Quang        | Review code của teammates khó vì thiếu docstring/explanation, dễ miss bug.                                              | Reviewer, teammates, team lead                                                                  | Reviewer phải đọc line-by-line để hiểu intent.                                                                | Có AI fit tốt, nhưng cần code repo thật để validate.                                                  |
| 6   | Quang        | Test local fail do config environment không đồng nhất giữa máy các thành viên.                                          | Developer/team/CI                                                                               | Debug config lặp lại sau pull/clone/switch branch.                                                            | Có vẻ Rule/Docker/Makefile có thể đủ, không nhất thiết cần AI.                                        |
| 7   | An           | Debug lỗi giữa frontend, backend và database mất thời gian vì phải kiểm tra nhiều layer.                                | Full-stack developer                                                                            | Xác định root cause giữa request, response, backend log và database.                                          | Workflow rõ, AI workflow có thể hỗ trợ, cần baseline thời gian/lỗi.                                   |
| 8   | An           | Khi nhận bug/feature, developer mất thời gian tìm đúng file/module cần sửa trong codebase lớn.                          | Developer                                                                                       | Search nhiều file và đọc dependency trước khi sửa.                                                            | Gần với coding agent use case, nhưng cần repo cụ thể để demo/validate.                                |
| 9   | An           | Thành viên hỏi lại cách setup/chạy project vì tài liệu setup chưa dễ dùng.                                              | Team member/developer                                                                           | Setup knowledge nằm rải rác hoặc chưa chuẩn hóa.                                                              | Process/docs có thể giải quyết trước; AI chỉ cần nếu project phức tạp.                                |
| 10  | Quân         | Task mới qua Messenger không có owner rõ, bị trôi và có thể bị quên.                                                    | Team lead và thành viên nhóm                                                                    | Không có bước xác nhận owner và danh sách task chưa được nhận.                                                | Rất mạnh cho group workflow; actor, bottleneck, metric đều rõ.                                        |
| 11  | Quân         | Thành viên hiểu sai task vì chi tiết nằm trong nhiều tin nhắn, dẫn đến rework.                                          | Người implement và lead review                                                                  | Không có task brief được xác nhận với goal, scope, workflow, acceptance criteria.                             | Pain thật, dễ validate với chat/task history, rất hợp bài toán nhóm.                                  |
| 12  | Quân         | Thành viên implement trùng scope vì owner/status/scope không nằm ở một source of truth.                                 | Team lead và các dev                                                                            | Thiếu liên kết giữa task, owner, branch/PR, status và deliverable.                                            | Impact rõ nhưng có thể là biến thể của task ownership/source of truth.                                |
| 13  | Đạt          | Business gửi ad-hoc data request mập mờ qua Slack, DA phải hỏi lại nhiều lần.                                           | Fresher DA và stakeholder                                                                       | Làm rõ time range, metric, filter, logic lọc qua nhiều tin nhắn.                                              | Metric tốt, workflow rõ, AI workflow hợp, nhưng domain DA riêng hơn.                                  |
| 14  | Đạt          | Fresher DA mất 60-90 phút debug SQL dài kế thừa khi dashboard lệch số.                                                  | Fresher DA/senior DA                                                                            | Đọc hiểu nhiều CTE/JOIN không có comment, phải bóc tách từng bước.                                            | AI fit cao, metric tốt, nhưng cần query thật và data context để validate.                             |
| 15  | Đạt          | Chuyển business request thành SQL draft mất 30-45 phút và dễ sai logic.                                                 | Fresher DA/business stakeholder                                                                 | Dịch yêu cầu kinh doanh sang bảng, join, filter và SQL logic.                                                 | Có thể mạnh nếu nhóm chọn DA domain, rủi ro hallucinate schema.                                       |
| 16  | Chương       | Sinh viên và khách đến VinUni khó tìm phòng học/hội trường và quán ăn quanh Ocean Park vì thông tin vị trí bị phân tán. | Tân sinh viên, sinh viên trường khác, giảng viên thỉnh giảng, khách tham quan, sinh viên VinUni | Google Maps không đủ indoor map từng tầng; phải đi lòng vòng/hỏi bảo vệ hoặc tự lướt nhiều nguồn để tìm quán. | Nhóm chọn làm final vì actor rộng, pain dễ hiểu, có bối cảnh VinUni thật và có metric 15-20 phút/lần. |
| 17  | Chương       | Người mua hàng online tốn nhiều thời gian so sánh giá và đọc review để lọc seeding, lỗi sản phẩm và rủi ro hàng kém chất lượng. | Người mua sắm trên Shopee, Lazada, TikTok Shop                                                 | Phải mở 3-5 gian hàng, đọc 20-30 review 1-2 sao và tự phân biệt lỗi thật với seeding hoặc lỗi vận chuyển.    | Workflow và metric khá rõ, AI fit tốt, nhưng domain shopping riêng hơn và có rủi ro crawl dữ liệu sàn. |
| 18  | Chương       | Người lớn tuổi gặp lỗi smartphone nhưng khó diễn đạt thuật ngữ kỹ thuật, còn con cháu hỗ trợ từ xa không nhìn thấy màn hình. | Người cao tuổi dùng smartphone và con cháu hỗ trợ kỹ thuật từ xa                              | Người lớn tuổi phải đi hỏi người xung quanh hoặc gọi con cháu nhưng mô tả lỗi không rõ.                      | Có giá trị nhân văn, nhưng card còn metric yếu và triển khai trên điện thoại khó hơn trong lab.        |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A - Learning overload / knowledge retrieval | Duy #1, Duy #2 | Người học bị quá tải vì kiến thức và tài liệu nằm rải rác; khó biết phần nào đã hiểu/chưa hiểu hoặc tìm lại đúng nguồn. | Gần nhất với bối cảnh khóa AI hiện tại. Cần đo bằng quiz/checklist hoặc time log tìm tài liệu. |
| B - Team task coordination / source of truth | Duy #3, Quân #1, Quân #2, Quân #3 | Nhóm làm việc qua chat/GitHub nhưng task thiếu owner, scope, status, brief và deliverable chính thức. | Cluster mạnh nhất về teamwork; nhiều thành viên có pain tương tự. Có thể validate bằng task/chat history. |
| C - Developer workflow / debugging / code review | Quang #2, Quang #3, An #1, An #2, An #3 | Developer mất thời gian hiểu code, debug nhiều layer, setup môi trường hoặc review PR. | Hợp với coding agent, nhưng cần repo/test/log cụ thể để đo. |
| D - Data analyst request / SQL workflow | Đạt #1, Đạt #2, Đạt #3 | DA mất thời gian làm rõ request, đọc/debug SQL cũ và chuyển business logic thành SQL. | Metric khá rõ, AI fit tốt, nhưng domain hơi riêng so với cả nhóm nếu không ai khác làm DA. |
| E - Weekly reporting | Quang #1 | Từ nhiều nguồn raw data, người làm phải viết lại thành progress narrative. | Metric rõ, nhưng candidate này đứng một mình, ít trùng với các bài khác. |
| F - Campus navigation / student daily utility | Chương #1 | Người mới hoặc khách ở VinUni khó tìm đúng phòng/tầng/lối đi, rồi tiếp tục mất thời gian tìm tiện nghi/quán ăn quanh trường. | Bối cảnh rất local, dễ demo bằng VinUni/Ocean Park, actor rộng hơn một nhóm học. |
| G - Online shopping review / decision support | Chương #2 | Người mua hàng online phải so sánh giá, đọc nhiều review và tự lọc review ảo trước khi mua. | Có metric thời gian rõ, nhưng phụ thuộc dữ liệu từ sàn TMĐT và không liên quan trực tiếp đến VinUni/lab. |
| H - Elderly mobile support | Chương #3 | Người lớn tuổi gặp lỗi điện thoại nhưng khó mô tả vấn đề; người hỗ trợ từ xa không nhìn thấy màn hình. | Pain dễ đồng cảm, nhưng metric và workflow trong file cá nhân còn mỏng nên khó chọn làm final ngay. |

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

Team task coordination có nhiều người gặp và score cao, nhưng có rủi ro là GitHub Issues/template/process fix đã giải quyết được phần lớn mà chưa cần AI. Developer debug/code navigation và DA request/SQL đều có AI fit tốt, nhưng cần dữ liệu thật như repo/log/SQL/schema để defend chắc hơn trong thời gian lab. Weekly reporting có metric rõ nhưng ít trùng với các thành viên khác. Hai idea còn lại của Chương là shopping review và hỗ trợ người lớn tuổi dùng smartphone đều có pain thật, nhưng một bài lệch khỏi bối cảnh nhóm/campus, một bài còn thiếu metric cụ thể để defend nhanh.
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
| Interview | Chưa thực hiện | Chưa có quote người dùng nên **không kết luận** pain đã được xác nhận. | Chưa có dữ liệu phản bác. | Thu hẹp bản thử nghiệm về việc tìm **phòng học/hội trường trong VinUni**; chỉ giữ phần quán ăn là mở rộng nếu người được hỏi nêu đây là nhu cầu lặp lại. |
| Micro-survey | Chưa thực hiện (mục tiêu: 5-10 người) | Cần thu câu trả lời nguyên văn cho: "Lần gần nhất bạn tìm phòng ở VinUni là khi nào? Bước nào khó nhất? Mất bao lâu? Bạn đã làm gì?" | Cần ghi cả trường hợp người trả lời tìm được ngay bằng biển chỉ dẫn, Google Maps hoặc hỏi lễ tân. | Chỉ giữ giả thuyết nếu đa số mẫu nêu khó khăn ở việc xác định đúng tòa/tầng/phòng hoặc lộ trình; nếu không, chuyển trọng tâm sang chuẩn hóa biển chỉ dẫn/directory thay vì xây sản phẩm AI. |
| Log / ticket / review | Chưa có | Không có log hỗ trợ, ticket hay số liệu thời gian đã được cung cấp để dùng làm bằng chứng. | - | Không dùng các con số "15-20 phút" hoặc "20-30 phút" ở các phần trước như số liệu đã kiểm chứng; xem đây là giả định cần đo trong pilot. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Trạng thái hiện tại: Not Yet - nhóm mới có giả thuyết hợp lý từ quan sát ban đầu, chưa có dữ liệu người dùng đủ để xác nhận. Nếu giả thuyết đúng, pain cốt lõi không phải là "thiếu một app bản đồ" mà là thiếu một nguồn thông tin đáng tin cậy nối mã phòng với tòa nhà, tầng và lộ trình; thông tin quán ăn là nhu cầu phụ cần kiểm chứng riêng.
```

**Kế hoạch hoàn tất validation trước khi nộp:** phỏng vấn 3 người thuộc ít nhất 2 nhóm (tân sinh viên/khách/sinh viên hiện tại); ghi nguyên văn 1 câu mỗi người, thời điểm gần nhất gặp vấn đề, cách xử lý hiện tại và thời gian ước lượng. Đính kèm ảnh poll hoặc ghi chú đã ẩn danh tại `02-group-problem-statement-interview-notes.md`. Không thay thế dữ liệu này bằng câu trả lời do AI tạo.

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Google Maps - Indoor Maps | [Google Maps Help: indoor maps](https://support.google.com/maps/answer/2803784?hl=en-GB) | Hiển thị sơ đồ tầng và cho chọn level ở các địa điểm có dữ liệu indoor map; hỗ trợ tìm POI trong tòa nhà. | Người dùng đã quen thuộc; giảm nhu cầu tạo một bản đồ nền mới. | Floor plan chỉ có ở địa điểm được hỗ trợ; nhóm chưa xác minh VinUni có dữ liệu phòng/tầng đầy đủ. Google Maps cũng không tự bảo đảm mã phòng, lối đi nội bộ hay trạng thái thay đổi tại campus. | Kiểm tra Google Maps trước khi build. Nếu dữ liệu VinUni thiếu, dùng Google Maps cho chỉ dẫn đến campus/tòa nhà, còn dữ liệu phòng và lộ trình nội bộ phải do nguồn được VinUni xác thực cung cấp. |
| ArcGIS Indoors Viewer | [ArcGIS Indoors: Viewer](https://doc.arcgis.com/en/indoors/latest/viewer/introduction-to-indoor-viewer.htm) | Tìm vị trí/tài nguyên trong tòa nhà hoặc nhiều tòa nhà; có thể định tuyến giữa các điểm và hỗ trợ chế độ kiosk cho khách. | Cho thấy mô hình campus-level cần room directory, map theo tầng và wayfinding - không chỉ search địa điểm. | Cần dữ liệu indoor được chuẩn hóa, vận hành/cập nhật và giấy phép ArcGIS; quá nặng cho pilot sinh viên. | Mượn pattern "tìm phòng -> xem tầng -> xem đường đi", nhưng pilot nên là web directory/map tĩnh có owner dữ liệu, không triển khai nền tảng enterprise. |
| OpenStreetMap - Simple Indoor Tagging | [Simple Indoor Tagging](https://wiki.openstreetmap.org/wiki/Simple_Indoor_Tagging) | Mô hình hóa tầng, phòng, hành lang và mã phòng (`level`, `ref`, `indoor=room/corridor`) để hiển thị/định tuyến indoor. | Làm rõ dữ liệu tối thiểu cần có: mã phòng, tầng, hành lang/lối nối và POI; có thể bắt đầu từ dữ liệu thô rồi tăng dần độ chi tiết. | Đây là quy ước dữ liệu cộng đồng, không tự tạo route hay bảo đảm dữ liệu chính xác; dữ liệu nội bộ có thể không phù hợp để công khai. | Thiết kế schema tối thiểu do VinUni quản trị: `building`, `floor`, `room_code`, `room_name`, `category`, `last_verified`; chỉ công bố thông tin được phép và có ngày kiểm tra. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nên bắt đầu bằng MVP không-AI: một directory phòng đã được xác thực, tìm theo mã phòng, hiển thị tòa/tầng và sơ đồ/lộ trình đơn giản; Google Maps chỉ dùng cho chặng ngoài trời hoặc khi indoor data của VinUni đã được kiểm tra. Không nên hứa hẹn định vị vị trí thời gian thực, tự tạo indoor route bằng AI, hay dữ liệu quán ăn/giờ mở cửa nếu chưa có owner cập nhật.

AI, nếu được dùng ở phase sau, chỉ nên hỗ trợ hiểu câu hỏi tự do (ví dụ: "A303 ở đâu?") rồi trả về bản ghi đã xác thực; AI không được suy đoán vị trí phòng hay giờ mở cửa. Điều kiện Go là có nguồn dữ liệu được VinUni xác nhận, owner cập nhật và kết quả quick validation cho thấy directory hiện tại chưa đủ.
```

> Nguồn đã kiểm: Google Maps Help, ArcGIS Docs và OpenStreetMap Wiki (truy cập 12/09/2026). Research cho thấy các pattern khả thi, **không** là bằng chứng rằng người dùng VinUni đang gặp pain này. Các giả định chưa kiểm chứng: mức độ đầy đủ của indoor map VinUni, thời gian tìm phòng, nhu cầu quán ăn, và quyền sử dụng/công bố sơ đồ campus.

---

# Phase 5 — Workflow + Problem Statement

## 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
CURRENT STATE — khoảng 15–20 phút tìm kiếm/xác nhận

[1 Nhận mã phòng hoặc phát sinh nhu cầu tìm quán: 1' - người dùng]
→ [2 Mở Google Maps/mạng xã hội: 2' - người dùng]
→ [3 Đọc và so sánh thông tin phân tán: 4–5' - người dùng]
→ [4 Hỏi bảo vệ/sinh viên hoặc gọi quán: 4–5' - người dùng] <-- bottleneck
→ [5 Đi thử, phát hiện sai đường/thông tin cũ và tìm lại: 5–7' - người dùng] <-- bottleneck
→ [6 Đến đúng phòng hoặc chọn được quán phù hợp]
```

> Thời gian trên là ước lượng ban đầu từ Problem Card, chưa phải kết quả validation chính thức. Thời gian đo là phần tìm kiếm, xác nhận và đi sai đường; không tính thời gian đi bộ đúng tuyến.

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Sinh viên/khách/giảng viên | Mã phòng, tên hội trường hoặc nhu cầu ăn uống | Nhu cầu tìm kiếm ban đầu | Khoảng 1 phút; thường xảy ra đầu học kỳ, khi đổi phòng hoặc giờ trưa | Mã phòng có thể ngắn và khó hiểu |
| 2 | Người dùng | Mã phòng hoặc từ khóa quán ăn | Kết quả Google Maps, bài đăng hoặc review | Khoảng 2 phút/lần | Google Maps thường chỉ đưa người dùng đến tòa nhà, chưa chắc có hướng dẫn chi tiết trong từng tầng |
| 3 | Người dùng | Nhiều kết quả từ các nguồn khác nhau | Danh sách vị trí có thể phù hợp | Khoảng 4–5 phút/lần | Thông tin phân tán; tên phòng, menu và giờ mở cửa có thể không đồng nhất |
| 4 | Người dùng, bảo vệ, sinh viên khác hoặc nhân viên quán | Câu hỏi về vị trí hoặc trạng thái quán | Hướng dẫn miệng hoặc xác nhận qua điện thoại | Khoảng 4–5 phút/lần | Bottleneck chính; phụ thuộc người khác có mặt và biết thông tin |
| 5 | Người dùng | Hướng dẫn chưa được xác nhận hoàn toàn | Tiếp tục đi hoặc phải tìm lại | Khoảng 5–7 phút/lần | Bottleneck; có thể đi sai tầng, sai lối hoặc tới quán đã đóng/chật |
| 6 | Người dùng | Vị trí cuối cùng đã được xác nhận | Đến đúng phòng hoặc chọn được quán | Tổng thời gian tìm kiếm khoảng 15–20 phút | Có nguy cơ trễ lớp hoặc mất nhiều thời gian nghỉ trưa |
| 7 | Không áp dụng | Không áp dụng | Không áp dụng | Không áp dụng | Workflow hiện tại chỉ cần 6 bước |

**Bottleneck chính (2-3 câu):**

```text
Bottleneck chính nằm ở bước xác nhận vị trí và tình trạng điểm đến. Không có một nguồn thống nhất chứa mã phòng, tầng, lối đi và dữ liệu tiện nghi nên người dùng phải hỏi người khác hoặc kiểm tra nhiều nguồn.

Phần này có thể chiếm khoảng 9–12 phút trong tổng thời gian tìm kiếm. Tuy nhiên đây mới là ước lượng ban đầu và nhóm cần bấm giờ hoặc phỏng vấn người dùng để xác nhận.
```

## 5.2. Future workflow bản nhóm

```text
FUTURE STATE — mục tiêu dưới 4 phút để nhận hướng dẫn có thể dùng

[1 Nhập mã phòng/tên địa điểm hoặc nhu cầu ăn uống: 30s - người dùng]
→ [2 Phân loại nhu cầu và chuẩn hóa từ khóa: <5s - Rule]
→ [3 Truy xuất dữ liệu phòng hoặc địa điểm phù hợp: 10–30s - Workflow/tool]
→ [4 AI tổng hợp hướng dẫn hoặc xếp hạng lựa chọn: 10–30s - AI]
→ [5 Xem nguồn, bản đồ và xác nhận lựa chọn: 30–60s - người dùng] <-- human boundary
→ [6 Mở lộ trình/bản đồ chính thức: <10s - máy]

Fallback: Nếu hệ thống không tìm thấy dữ liệu hoặc độ tin cậy thấp, không tự đoán. Hệ thống hiển thị file PDF sơ đồ chính thức, vị trí quầy bảo vệ gần nhất hoặc nút gọi quán. Người dùng có thể báo sai để người quản trị cập nhật dữ liệu.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian tìm kiếm và xác nhận | Khoảng 15–20 phút | Dưới 4 phút | Bấm giờ từ lúc nhận mã phòng/nhập nhu cầu đến khi có hướng dẫn được người dùng chấp nhận |
| Thời gian từ câu hỏi đến hướng dẫn đầu tiên | Chưa đo riêng | Dưới 2 phút | Ghi timestamp lúc gửi câu hỏi và lúc kết quả xuất hiện |
| Số bước | 6 bước | 5–6 bước ngắn | Đếm các bước người dùng phải thực hiện |
| Số bước thủ công | Khoảng 5 bước | Khoảng 2 bước | Đếm thao tác cần người dùng tự tìm, so sánh hoặc hỏi người khác |
| Tỷ lệ tìm đúng phòng/lựa chọn đúng ngay lần đầu | Chưa có baseline | Ít nhất 90% trong pilot | Giao nhiệm vụ tìm phòng rồi kiểm tra kết quả thực tế |
| Tỷ lệ phải hỏi trực tiếp | Chưa có baseline | Giảm ít nhất 80% | Hỏi người tham gia có cần nhờ bảo vệ/sinh viên khác không |
| Bottleneck chính | Xác nhận thủ công từ nhiều nguồn | Chất lượng và độ mới của dữ liệu | Theo dõi câu trả lời thiếu dữ liệu, sai phòng hoặc sai giờ mở cửa |
| Risk mới | Không có câu trả lời tập trung | AI chỉ sai đường hoặc dùng dữ liệu cũ | Lưu feedback, kiểm tra nguồn và đánh dấu kết quả có độ tin cậy thấp |

## 5.3. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Actor chính là tân sinh viên, sinh viên trường khác, giảng viên thỉnh giảng và khách lần đầu đến VinUni. Sinh viên hiện tại cũng gặp vấn đề khi phòng học hoặc địa điểm thay đổi. |
| **Workflow** | Người dùng nhận mã phòng hoặc có nhu cầu tìm tiện nghi, sau đó tìm trên Google Maps, mạng xã hội hoặc hỏi người xung quanh. Họ phải tự ghép thông tin rồi đi thử đến địa điểm. |
| **Bottleneck** | Thông tin mã phòng, tầng, lối đi và tiện nghi chưa nằm trong một nguồn dễ tra cứu. Người dùng mất nhiều thời gian nhất ở bước kiểm tra thông tin và hỏi người khác. |
| **Impact** | Người dùng có thể trễ lớp, lỡ điểm danh hoặc mất 20–30 phút nghỉ trưa. Người mới cũng cảm thấy bối rối và có trải nghiệm không tốt khi đến campus. |
| **Success Metric** | Mục tiêu là đưa hướng dẫn đầu tiên trong dưới 2 phút và hoàn tất việc tìm kiếm/xác nhận trong dưới 4 phút. Pilot hướng tới tỷ lệ tìm đúng ngay lần đầu ít nhất 90% và giảm ít nhất 80% số trường hợp phải hỏi trực tiếp. |
| **Boundary** | Hệ thống hỗ trợ tra cứu và đề xuất, nhưng người dùng vẫn kiểm tra bản đồ hoặc nguồn trước khi di chuyển. Hệ thống không được tự đoán khi thiếu dữ liệu và không bảo đảm quán còn bàn trống theo thời gian thực. |

**Câu hỏi AI phản biện v0 (nếu có):**

- Field nào mơ hồ: Problem đang ghép hai workflow là tìm phòng và tìm quán ăn. Baseline 15–20 phút cũng chưa được xác nhận bằng bấm giờ hoặc khảo sát.
- Tôi sửa gì: Chọn tìm phòng VinUni làm MVP chính. Quán ăn quanh Ocean Park là nhánh mở rộng sau khi MVP đã có dữ liệu và kết quả pilot.

---

# Phase 6 — Rule / Workflow / Agent + Decision

## 6.0. Ma trận độ phù hợp

- Độ mơ hồ: [ ] Thấp / [x] Cao — Vì sao: Người dùng có thể nhập mã phòng, tên viết tắt, mô tả sự kiện hoặc yêu cầu quán ăn bằng ngôn ngữ tự nhiên. Tuy nhiên vị trí phòng sau khi xác định đúng mã là dữ liệu có đúng/sai khá rõ.
- Độ phức tạp: [ ] Thấp / [x] Cao — Vì sao: Hệ thống có nhiều nguồn dữ liệu và phải rẽ nhánh giữa tìm phòng với tìm tiện nghi. Mỗi nhánh có cách truy xuất và tiêu chí kiểm tra khác nhau.

**Bài toán nhóm nằm ở ô nào:**

```text
Độ mơ hồ cao – Độ phức tạp cao, nhưng có thể giới hạn thành một Workflow có các bước và nhánh được xác định trước.
```

**Vì sao (2-3 câu):**

```text
Câu hỏi của người dùng có nhiều cách diễn đạt và đôi khi thiếu mã phòng hoặc tiêu chí lựa chọn. Hệ thống cũng phải lấy dữ liệu từ sơ đồ nội khu, danh sách phòng và nguồn địa điểm bên ngoài.

Tuy nhiên các hành động chính vẫn có thể thiết kế trước. Vì vậy nhóm chưa cần một Agent tự lập kế hoạch hoàn toàn.
```

## 6.1. So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Dùng bảng ánh xạ mã phòng → tòa → tầng → sơ đồ; dùng điều kiện giờ mở cửa và khoảng cách để lọc quán | Đủ khi người dùng nhập đúng mã phòng hoặc chọn từ danh sách có sẵn | Không hiểu tốt lỗi chính tả, tên gọi không chính thức hoặc yêu cầu tự nhiên | Có dùng cho chuẩn hóa mã phòng, kiểm tra dữ liệu và lọc điều kiện cứng |
| **Workflow** | Phân loại nhu cầu → lấy dữ liệu từ nguồn phù hợp → xếp hạng → tạo hướng dẫn → người dùng xác nhận | Phù hợp với MVP vì các bước và nhánh đã biết trước | Nếu dữ liệu sai hoặc cũ thì toàn bộ kết quả sau đó cũng có thể sai | **Chọn làm mức chính** |
| **Agent** | Agent tự chọn công cụ, tìm thêm nguồn, thay đổi kế hoạch và gọi nhiều API cho đến khi có câu trả lời | Chỉ cần khi truy vấn rất mở, thiếu dữ liệu và cần tự tìm nhiều nguồn động | Khó kiểm soát, tốn chi phí, có thể chọn nguồn kém tin cậy hoặc tự suy đoán | Chưa chọn cho MVP; chỉ cân nhắc ở phiên bản sau |

**5 câu hỏi chốt:**

1. **Rule có giải được 70–80% case không?**  
   Rule có thể giải quyết khoảng 70–80% trường hợp tìm phòng nếu người dùng nhập đúng mã và nhóm có bảng dữ liệu phòng đầy đủ. Rule không đủ cho lỗi chính tả, tên gọi không chính thức và yêu cầu quán ăn có nhiều tiêu chí.

2. **Các bước có đi thẳng một đường không hay phải rẽ nhánh?**  
   Workflow phải rẽ nhánh sau khi xác định người dùng muốn tìm phòng hay tìm tiện nghi. Sau đó mỗi nhánh vẫn đi theo một chuỗi bước khá cố định.

3. **Có thật sự cần Agent tự lập kế hoạch + gọi tool không?**  
   Chưa cần trong MVP. Workflow có thể gọi đúng nguồn theo từng nhánh mà không cần Agent tự quyết định kế hoạch dài hoặc tự thực hiện hành động ngoài yêu cầu.

4. **Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?**  
   Người dùng là người phát hiện đầu tiên khi hướng dẫn không khớp với sơ đồ hoặc địa điểm thực tế. Họ có thể chuyển sang PDF/hỏi bảo vệ ngay trong khoảng một phút; nhóm quản trị dữ liệu cần kiểm tra và sửa bản ghi được báo sai trong vòng 24 giờ.

5. **Có hạ được từ Agent → Workflow → Rule không?**  
   Có. MVP nên hạ xuống Workflow; riêng việc ánh xạ một mã phòng chính xác có thể tiếp tục hạ xuống Rule để tăng độ ổn định.

**Mức chọn:**

```text
Workflow
```

**Vì sao chọn (3-4 câu):**

```text
Bài toán có nhiều bước và hai nhánh dữ liệu, nhưng đường đi của mỗi nhánh có thể xác định trước. Workflow đủ để phân loại yêu cầu, lấy dữ liệu, tạo hướng dẫn và yêu cầu người dùng xác nhận.

AI chỉ nên hỗ trợ hiểu câu hỏi và trình bày kết quả. Dữ liệu vị trí phải đến từ bảng phòng và sơ đồ đã được xác nhận, không để AI tự tạo.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Rule thuần túy phù hợp với mã phòng chính xác nhưng khó xử lý lỗi chính tả, tên gọi không chính thức và yêu cầu bằng ngôn ngữ tự nhiên. Nó cũng khó xếp hạng quán ăn theo nhiều tiêu chí cùng lúc.

Tuy nhiên Rule vẫn được giữ bên trong Workflow cho những phần có đúng/sai rõ như ánh xạ mã phòng và kiểm tra giờ mở cửa.
```

## 6.2. Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Actor chính của MVP là tân sinh viên, khách và giảng viên thỉnh giảng cần tìm phòng hoặc hội trường trong VinUni. Sinh viên hiện tại là actor phụ khi có đổi phòng hoặc tham gia sự kiện ở khu vực chưa quen. |
| **Workflow** | Người dùng nhận mã phòng, tìm bằng Google Maps rồi hỏi bảo vệ hoặc sinh viên khác vì thiếu chỉ dẫn từng tầng. MVP cho phép họ nhập mã/tên phòng, nhận tòa, tầng, lối đi và mở sơ đồ nguồn để kiểm tra. |
| **Bottleneck** | Bước tốn thời gian nhất là chuyển từ mã phòng sang một lộ trình nội khu có thể sử dụng. Thông tin hiện bị phân tán và việc xác nhận phụ thuộc vào người khác. |
| **Impact** | Người dùng có thể mất khoảng 15–20 phút tìm kiếm và đi sai đường, dẫn đến trễ lớp hoặc lỡ điểm danh. Con số này đang là ước lượng và cần validation trước khi dùng như baseline chính thức. |
| **Success Metric** | Hướng dẫn đầu tiên xuất hiện trong dưới 2 phút; tổng thời gian tìm kiếm/xác nhận dưới 4 phút; tỷ lệ tìm đúng ngay lần đầu ít nhất 90%. Tỷ lệ phải hỏi trực tiếp giảm ít nhất 80% trong pilot. |
| **Boundary (làm / không làm)** | MVP làm tra cứu phòng, tòa, tầng, lối đi và hiển thị sơ đồ nguồn. MVP chưa làm định vị indoor theo thời gian thực, không bảo đảm tình trạng bàn trống và không tự đặt bàn hoặc thanh toán; tìm quán chỉ là extension. |
| **AI intervention point** | AI can thiệp sau khi hệ thống nhận câu hỏi và trước khi kết quả được hiển thị. AI chuẩn hóa cách hỏi, chọn từ các bản ghi đã truy xuất và tạo hướng dẫn dễ đọc; AI không được tự tạo vị trí không có trong dữ liệu. |
| **Mức chọn** | Workflow — vì bài toán cần nhiều bước và có rẽ nhánh nhưng chưa cần Agent tự lập kế hoạch. |
| **Rủi ro & người thật kiểm tra** | Rủi ro lớn nhất là sơ đồ cũ hoặc AI chỉ sai tầng/lối đi. Người dùng kiểm tra bản đồ nguồn trước khi di chuyển; một thành viên nhóm hoặc đầu mối quản trị kiểm tra các báo cáo sai và cập nhật dữ liệu. |

## 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor chính và workflow tìm phòng đã rõ; tìm quán được chuyển thành extension. |
| Baseline + metric đo được chưa? | Not Yet | Nhóm có ước lượng 15–20 phút nhưng chưa có log bấm giờ, interview hoặc survey để xác nhận. |
| Data/input đủ dùng chưa? | Not Yet | Nhóm chưa xác nhận quyền sử dụng sơ đồ tầng, danh sách mã phòng và mức độ đầy đủ của dữ liệu. |
| AI sai, hậu quả chấp nhận được không? | Yes, có điều kiện | Có thể chấp nhận trong pilot nhỏ nếu luôn hiển thị nguồn và có fallback; không được dùng AI để tự đoán vị trí. |
| Có người review/owner không? | Not Yet | Nhóm cần chỉ định một thành viên chịu trách nhiệm kiểm tra sơ đồ, danh sách phòng và feedback. |
| Có cách non-AI đơn giản hơn không? | Yes | Một trang tìm kiếm mã phòng, bảng dữ liệu hoặc PDF có QR code có thể giải quyết phần lớn trường hợp cơ bản. |

**Decision:**

```text
Not Yet
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Problem có actor và workflow rõ, nhưng baseline 15–20 phút hiện mới là ước lượng từ Problem Card. Nhóm cũng chưa xác nhận có sơ đồ chính thức và danh sách phòng đủ sạch để tạo hướng dẫn chính xác.

AI không thể bù cho dữ liệu vị trí bị thiếu hoặc sai. Vì vậy nhóm nên validation và chuẩn bị một tập dữ liệu nhỏ trước, sau đó mới Go với pilot giới hạn.
```

**Nếu Go — pilot nhỏ nhất:**

```text
Chưa Go ngay. Sau khi đủ điều kiện, pilot chỉ nên dùng một tòa hoặc một tầng với khoảng 20–30 phòng đã được kiểm tra bằng sơ đồ chính thức.

Nhóm có thể lưu mã phòng, tầng, mốc rẽ và đường dẫn sơ đồ trong Google Sheets/JSON. Workflow được chạy thử bằng chatbot đơn giản, chưa cần Agent và chưa cần định vị indoor theo thời gian thực.

Ba số cần đo:
1. Thời gian trung vị từ lúc nhập mã phòng đến khi nhận hướng dẫn có thể dùng.
2. Tỷ lệ người dùng xác định hoặc tìm đúng phòng ngay lần đầu.
3. Tỷ lệ người dùng vẫn phải hỏi bảo vệ hoặc sinh viên khác.
```

**Nếu Not Yet — cần validate gì trước:**

```text
1. Phỏng vấn 3 người mới đến VinUni và ghi lại câu nói nguyên văn.
2. Cho 5–10 người thực hiện nhiệm vụ tìm 2–3 phòng rồi bấm giờ để có baseline thật.
3. Xác nhận nhóm có thể sử dụng sơ đồ chính thức và tạo danh sách mã phòng cho khu vực pilot.
4. So sánh prototype AI với một phương án non-AI gồm bảng tìm kiếm phòng và PDF có QR code.
5. Chỉ định một data owner chịu trách nhiệm kiểm tra và cập nhật thông tin.
```

**Nếu No-Go — làm gì thay AI:**

```text
Không áp dụng vì quyết định hiện tại là Not Yet, không phải No-Go. Nếu dữ liệu không đủ để làm AI, nhóm có thể tạo một trang tra cứu mã phòng đơn giản kết hợp QR code dẫn tới PDF sơ đồ chính thức.
```
