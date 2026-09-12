# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Nguyễn Hữu Chương
- Mã học viên: 2A202602601
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm cuối
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):Nấu ăn, đọc tài liệu, mua hàng,...

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 |Lặp lại |Nghĩ thực đơn nấu ăn |Người nội trợ|Thường suy nghĩ "Hôm nay ăn gì" |
| 2 | Tốn thời gian|So sánh giá, đọc review trước khi mua hàng |Người hay mua hàng online |Tìm sản phẩm trên các cửa hàng khác nhau, soi bình luận |
| 3 |Tốn thời gian |Tìm kiếm các lớp học trong Vinuni, các tiện ích xung quanh |Sinh viên, học viên mới, khách |Tìm kiếm từng địa điểm tham quan, chỗ ăn, ở và lộ trình phù hợp |
| 4 |AI có thể tốt hơn |Trả lời và tổng hợp thông tin trong 1 văn bản dài |Người dùng |Hỏi thông tin có trong file, tóm tắt thông tin |
| 5 | AI có thể tốt hơn|Dịch thuật |Người dùng |Đưa văn bản vào nhờ AI sửa lỗi hoặc dịch ngôn ngữ khác |
| 6 |Pain từ người khác |Hỗ trợ người lớn tuổi dùng các thiết bị di động|Con cháu|Sao không điện được,... |
| 7 |Lặp lại |Ghi lại chi tiêu |Người quản lý tài chính cá nhân |Ghi lại chi tiêu hàng ngày |
| 8 | Tốn thời gian|Xếp hàng đợi thang máy, đợi lấy cơm |Nhiều người |Hàng trăm người xếp hàng đợi nhận cơm trưa |

**AI đã dùng ở Phase 1 (nếu có):** Gemini
- Prompt đã hỏi: Dưới đây là 4 lăng kính để scan các vấn đề trong cuộc sống và 1 vài ví dụ. Hãy cho t các vấn đề theo định dạng bên dưới, với mỗi lăng kính cho t 3 vấn đề thường gặp trong cuộc sống thường ngày của mọi người...
- Ý dùng được: Nghĩ thực đơn nấu ăn, trả lời và tổng hợp thông tin trong văn bản dài,...
- Ý bỏ vì không phải pain thật:Lọc và xóa tin nhắn rác, email quảng cáo, Canh đặt lịch hẹn dịch vụ định kỳ (sân thể thao, bảo dưỡng xe, tái khám),...

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
| 1 |Tìm kiếm các lớp học trong Vinuni, các tiện ích xung quanh |Đề tài thực tế, cần kết hợp nhiều công cụ như Google Maps|Thông tin về các quán ăn uống có chính xác hay không |
| 2 |So sánh giá, đọc review trước khi mua hàng |Thực tế, tiết kiệm thời gian cho người mua hàng |Lấy được các bình luận của sản phẩm trên các sàn thương mại điện tử |
| 3 |Hỗ trợ người lớn tuổi dùng các thiết bị di động |Thực tế, giá trị nhân văn |Tích hợp được vào điện thoại |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Tìm kiếm phòng học trong VinUni và tiện ích xung quanh

```text
Problem 1:
Sinh viên và khách đến VinUni gặp khó khăn khi định vị phòng học/hội trường trong cụm tòa nhà phức tạp và mất nhiều thời gian tìm kiếm quán ăn phù hợp quanh khu vực Vinhomes Ocean Park do thông tin bị phân tán.
Actor: Tân sinh viên, sinh viên các trường khác đến giao lưu, giảng viên thỉnh giảng, khách tham quan và sinh viên nội khu VinUni.


Thời điểm / bối cảnh: Đầu học kỳ mới, các tuần thi/bảo vệ đồ án đổi phòng học đột xuất, hoặc khung giờ nghỉ trưa (11h30 – 13h00) cần tìm chỗ ăn nhanh gần trường.

Current workflow 3-7 bước:
1. Nhận thông tin mã phòng học trên lịch học (vd: C-201, Lab AI) hoặc có nhu cầu đi ăn trưa.
2. Mở Google Maps nhưng ứng dụng không hỗ trợ sơ đồ chi tiết từng tầng bên trong tòa nhà.
3. Đi bộ lòng vòng qua các sảnh, dừng lại hỏi bảo vệ hoặc sinh viên đi ngang qua để tìm đúng thang máy/lối rẽ.
4. Với việc ăn uống: mở app bản đồ hoặc mạng xã hội tìm quán ăn quanh Ocean Park, lướt xem menu và khoảng cách.
5. Đến nơi bị trễ giờ học, hoặc tới quán phát hiện quán đã đóng cửa/chật kín bàn.

Bottleneck: Bước 3 & 4 — Thiếu dữ liệu sơ đồ nội khu (indoor map) và thông tin giờ mở cửa thực tế của các quán ăn xung quanh bị phân mảnh, phụ thuộc vào việc hỏi đường thủ công (15–20 phút/lần).

Impact: Trễ giờ vào lớp, lỡ buổi điểm danh; lãng phí 20–30 phút nghỉ trưa quý giá; gây cảm giác lúng túng, bối rối cho người mới.

Success metric: Giảm thời gian tìm đúng vị trí phòng/quán ăn từ 20 phút xuống dưới 2 phút; giảm tỷ lệ phải dừng lại hỏi đường trực tiếp > 80%.

Non-AI alternative: Xem bản đồ, lập bảng Google Sheets tổng hợp vị trí, hotline các quán ăn xung quanh trường chia sẻ cho sinh viên.

AI hypothesis: Kết hợp RAG trên cơ sở dữ liệu sơ đồ VinUni với Google Maps/Search Tool, bổ sung thêm nguồn dữ liệu crawl trên mạng.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[*] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 20 phút

[1 Nhận mã phòng / Nhu cầu ăn: 1'] 
→ [2 Tra cứu Google Maps: 2'] 
→ [3 Đi lòng vòng & hỏi bảo vệ/sinh viên: 10'] <-- bottleneck
→ [3' Lướt tìm quán, check giờ mở cửa: 7']  <-- bottleneck

FUTURE STATE — 4 phút

[1 Nhập mã phòng hoặc gu ăn uống vào Bot: 1'] 
→ [2 Agent RAG sơ đồ tầng & truy vấn trạng thái quán: 2'] 
→ [3 Người dùng xem lộ trình & chọn quán: 1']  <-- human boundary

Fallback: Nếu AI chỉ sai vị trí phòng hoặc quán đã đóng cửa/đổi chỗ, hệ thống cung cấp sẵn nút bấm mở nhanh file PDF sơ đồ các tầng chính thức của VinUni và link bảng Google Sheets tổng hợp số hotline/trạng thái quán ăn do cộng đồng sinh viên cập nhật.

```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — So sánh giá và đọc review trước khi mua hàng online

```text
Problem 1 câu:
Người mua sắm trực tuyến tốn nhiều thời gian đọc thủ công hàng trăm bình luận trên các sàn thương mại điện tử để lọc review ảo (seeding) và tìm ra các lỗi hư hỏng/kém chất lượng tiềm ẩn của sản phẩm.

Actor:
Người tiêu dùng mua sắm thường xuyên trên Shopee, Lazada, TikTok Shop (nhóm khách hàng mua đồ công nghệ, đồ gia dụng, thời trang phân khúc từ vừa đến cao).

Thời điểm / bối cảnh:
Giai đoạn cân nhắc trước khi bấm thanh toán, đặc biệt vào các đợt Mega Sale (ngày đôi, sale lương về) khi áp lực chốt đơn nhanh để giữ mã giảm giá.

Current workflow 3-7 bước:
1.Gõ tìm tên sản phẩm trên sàn TMĐT.
2.Mở 3–5 gian hàng có lượt bán cao nhất để so sánh mức giá niêm yết.
3.Bấm vào mục Đánh giá, lọc riêng các bài 1 sao, 2 sao và các đánh giá có đính kèm hình ảnh/video thật.
4.Đọc thủ công 20–30 bình luận để phân biệt phản ánh lỗi do sản phẩm hay do đơn vị vận chuyển, kiểm tra xem có mẫu câu seeding lặp lại hay không.
5.Cân nhắc lại mức giá cuối cùng sau voucher rồi mới quyết định bấm mua hoặc từ bỏ vì quá mệt mỏi.

Bottleneck:Bước 3 & 4 — Đọc, chọn lọc và đối chiếu khối lượng văn bản lớn từ phản hồi người dùng; khó phát hiện seeding tinh vi (chiếm 25–30 phút/sản phẩm).

Impact: Ra quyết định mua sắm chậm; rủi ro mua phải hàng kém chất lượng dẫn đến khiếu nại, đổi trả phức tạp; mất tiền oan vào hàng giả.

Success metric: Giảm thời gian nghiên cứu sản phẩm từ 30 phút xuống dưới 3 phút; độ chính xác trong việc tóm tắt lỗi sản phẩm và phát hiện seeding đạt > 85\%.

Non-AI alternative: Tìm kiếm và so sánh thủ công

AI hypothesis: Sử dụng Search tool để tìm kiếm các sản phẩm trên mạng, Sentiment Analysis để thống kê phân tích các bình luận.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[*] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 30 phút

[1 Tìm & mở 3–5 gian hàng: 3'] 
→ [2 So sánh giá niêm yết: 2'] 
→ [3 Lọc & đọc thủ công 20–30 review 1–2 sao: 15'] 
→ [4 Soi mẫu câu seeding & bóc tách lỗi: 8']  <-- bottleneck 
→ [5 Cân nhắc áp voucher & chốt: 2']

FUTURE STATE — 7 phút

[1 Dán link hoặc tên sản phẩm vào tool: 2'] 
→ [2 AI crawl review, phân tích khía cạnh (ABSA) & lọc seeding: 3'] 
→ [3 Người dùng review bảng lỗi tổng hợp và chốt mua: 2']  <-- human boundary

Fallback: Nếu hệ thống bị sàn TMĐT chặn crawl dữ liệu bình luận, trả về sắp xếp giá theo kết quả tìm kiếm.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Hỗ trợ người lớn tuổi sử dụng thiết bị di động từ xa

```text
Problem 1 câu:
Người lớn tuổi gặp sự cố khi dùng smartphone nhưng không biết diễn đạt thuật ngữ kỹ thuật, trong khi con cháu hỗ trợ từ xa không nhìn thấy màn hình để hướng dẫn, dẫn đến bế tắc và căng thẳng giao tiếp.
Actor:
Người cao tuổi (ông bà, cha mẹ) sử dụng smartphone và con cháu làm việc/học tập xa nhà thường xuyên phải hỗ trợ kỹ thuật.
Thời điểm / bối cảnh:
Khi điện thoại bất ngờ bị mất kết nối mạng, âm lượng bị tắt, nhảy quảng cáo che màn hình, hoặc cần gọi video nhưng giao diện ứng dụng tự động cập nhật đổi nút bấm.

Current workflow 3-7 bước:
1.Người lớn tuổi gặp lỗi hoặc không biết thao tác tiếp trên màn hình điện thoại.
2.Đem đi hỏi hàng xóm.
3.Chờ đợi.
4.Hoàn thành.

Bottleneck: Đi hỏi người xung quanh

Impact: Tốn thời gian, ngại.

Success metric: Giảm thời gian.

Non-AI alternative: Đi hỏi mọi người.

AI hypothesis: Tích hợp mô hình AI nhận giọng nói người dùng vào điện thoại.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[*] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 11 phút

[1 Gặp lỗi, không biết thao tác tiếp: 1'] 
→ [2 Đi hỏi cầu cứu 10'] 


FUTURE STATE — 2.5 phút

[1 Vào app: 0.5'] 
→ [2 Voice để hỏi: 2'] <-- human boundary

Fallback: Nếu Vision AI không xác định được lỗi hoặc độ tự tin nhận diện tọa độ nút bấm thấp, phản hồi không trả lời được.".
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Tìm kiếm phòng học trong VinUni và tiện ích xung quanh

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Quy trình được chuẩn hóa từ chuỗi thao tác rời rạc (tra Maps thiếu dữ liệu nội khu → hỏi đường thủ công → lướt mạng tìm quán) thành một luồng Agent hợp nhất: truy xuất sơ đồ tầng (Indoor RAG) và tra cứu trạng thái quán ăn thực tế qua Maps/Search Tool.
Giải pháp giúp cắt giảm thời gian tìm đúng địa điểm từ 20 phút xuống dưới 4 phút, giảm hơn 80% tần suất người mới phải đi lòng vòng hỏi đường.
Tác động trực tiếp triệt tiêu nguy cơ trễ giờ lên lớp/giờ thi cho tân sinh viên và khách tham quan, đồng thời trả lại trọn vẹn quỹ thời gian nghỉ trưa vốn đã eo hẹp.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
Công nghệ có thực tế để triển khai hay không. Các nguồn để bổ sung dữ liệu.

```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Dữ liệu quán xá biến động liên tục.
- Tôi sửa gì: Bổ sung dữ liệu cào trên mạng, cho phép người dùng báo cáo các địa điểm sai để xóa.

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
