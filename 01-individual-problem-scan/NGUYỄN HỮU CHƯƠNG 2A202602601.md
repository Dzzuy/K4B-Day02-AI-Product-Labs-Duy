
#### Problem Card #1 — Tìm kiếm phòng học trong VinUni và tiện nghi xung quanh

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



