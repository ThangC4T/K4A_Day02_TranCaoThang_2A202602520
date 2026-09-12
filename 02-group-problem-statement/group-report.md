# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Nguyễn Duy Khánh | 2A202602736 | Facilitator, Writer |
| 2   | Nguyễn Triều Vương | 2A202602422 | Workflow Specialist |
| 3   | Trần Cao Thắng | 2A202602520 | Research Specialist |

**Candidate problem nhóm chọn (1 câu):**
Tự động hóa quy trình tra cứu danh sách, tạo tin nhắn Zalo cá nhân hóa và phân loại phản hồi nhắc lịch bảo dưỡng định kỳ cho đại lý VinFast bằng AI Workflow.

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Nguyễn Duy Khánh | Tra cứu danh sách và gửi tin nhắn/gọi điện nhắc lịch bảo dưỡng định kỳ cho từng khách hàng thủ công | Nhân viên CSKH (Khánh) & Khách hàng đi xe VinFast | Tra cứu Excel thủ công & nhắn/gọi từng người (tốn 120 phút/ngày, 15% nhầm lẫn mốc bảo dưỡng) | Workflow rất rõ ràng, pain lớn, baseline đo được bằng thời gian/doanh thu xưởng. Rất tiềm năng! |
| 2 | Nguyễn Duy Khánh | Trả lời lặp đi lặp lại các câu hỏi qua Zalo/Fanpage về bảng giá phụ tùng, chi phí bảo dưỡng định kỳ và giờ làm việc | Nhân viên CSKH & Khách hàng nhắn Zalo/Fanpage | Tra cứu bảng giá Excel thủ công cho từng loại xe (85 tin/tuần, khách chờ 15-25 phút) | Tần suất lặp lại cao, giải quyết dễ bằng Rule/Workflow tra cứu bảng giá. |
| 3 | Nguyễn Duy Khánh | Tra cứu tài liệu thể lệ và điều khoản bảo hành VinFast (dài hàng chục trang) để giải đáp thắc mắc phức tạp | Nhân viên CSKH, Cố vấn dịch vụ & Khách hàng | Đọc và đối chiếu quy định bảo hành PDF dài (10-15 phút/ca, rủi ro tư vấn sai) | Bài toán RAG hay, nhưng tần suất phát sinh ít hơn bài nhắc lịch bảo dưỡng. |
| 4 | Nguyễn Triều Vương | A lifeguard must continuously watch several swimmers and may not notice a possible drowning event immediately | Swimmers, lifeguards, and pool operators | Quan sát mắt thường liên tục dễ mất tập trung/kiệt sức (không nhận diện kịp thời sau 20-30 phút) | Pain cực lớn về an toàn tính mạng, nhưng cần hệ thống AI Camera đắt đỏ, khó triển khai pilot trong lab. |
| 5 | Nguyễn Triều Vương | Visitors queue while staff manually scan admission tickets at an amusement-park entrance | Visitors and gate staff | Quét mã từng vé thủ công vào giờ cao điểm (mất 15-30s/khách, dồn ứ hàng dài) | Quy trình đơn giản, giải quyết được bằng cổng đọc mã QR tự động (Rule/Hardware), chưa cần AI. |
| 6 | Nguyễn Triều Vương | Technical teams manually collect records and perform the same cable-car safety and performance checklist every week | Technical operations engineers and maintenance supervisors | Ghi chép và nhập liệu checklist thủ công từ hàng chục cảm biến cáp treo (mất 4-6 giờ/tuần, dễ bỏ sót chỉ số) | Quy trình chuẩn hóa cao, phù hợp ứng dụng AI/Rule phát hiện chỉ số bất thường. |
| 7 | Trần Cao Thắng | Tổng hợp và phân loại phản hồi (review/rating) của khách hàng từ Shopee, Facebook, Google Maps | Nhân viên Marketing, CSKH & Quản lý bán hàng | Đọc và gán nhãn tích cực/tiêu cực thủ công từng đánh giá (tốn 4-5 giờ/tuần) | Thích hợp làm Sentiment Analysis, nhưng impact không trực tiếp bằng việc hỗ trợ vận hành hàng ngày. |
| 8 | Trần Cao Thắng | Kiểm tra và đối chiếu các điều khoản phạt trong hợp đồng cung ứng dịch vụ B2B thủ công | Nhân viên Pháp chế, Sales & Khách hàng B2B | Đọc đối chiếu hợp đồng mẫu với yêu cầu riêng của khách (tốn 45 phút/hợp đồng) | Quy trình phức tạp, rủi ro pháp lý cao nếu AI trích xuất thiếu điều khoản. |
| 9 | Trần Cao Thắng | Phân loại và gán độ ưu tiên (Priority) cho ticket hỗ trợ kỹ thuật bị dồn đống chưa xử lý | Nhân viên IT Helpdesk & Khách hàng nội bộ | Đọc nội dung ticket để phân loại bộ phận xử lý thủ công (mất 10 phút/ticket, trễ KPI 20%) | Bài toán chuẩn hóa tốt, tuy nhiên chưa có dữ liệu thực tế tại đại lý bằng bài toán VinFast. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A | Candidate 1, Candidate 2, Candidate 9 | **Chăm sóc & Nhắc lịch dịch vụ khách hàng:** Thu thập thông tin lịch sử $\rightarrow$ Tra cứu quy trình/giá $\rightarrow$ Tạo thông điệp cá nhân hóa $\rightarrow$ Phân loại phản hồi | Nhóm bài toán có workflow tuyến tính rõ ràng, dễ đo lường trước/sau |
| B | Candidate 4, Candidate 6 | **Giám sát an toàn & Kiểm tra kỹ thuật tự động:** Theo dõi dữ liệu cảm biến/hình ảnh liên tục $\rightarrow$ Phát hiện chỉ số/hành vi bất thường $\rightarrow$ Cảnh báo | Yêu cầu tích hợp phần cứng cảm biến/camera, rủi ro an toàn cao |
| C | Candidate 3, Candidate 5, Candidate 7, Candidate 8 | **Xử lý thủ tục quầy & Tổng hợp báo cáo dữ liệu:** Đọc tài liệu/mã vé $\rightarrow$ Đối chiếu điều khoản/quy định $\rightarrow$ Trích xuất dữ liệu | Thiếu tính tương tác trực tiếp tạo ra giá trị doanh thu ngay cho cửa hàng |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| **Candidate 1: Nhắc lịch bảo dưỡng định kỳ qua Zalo/SMS** | 1. Workflow rõ ràng (Lọc dữ liệu $\rightarrow$ Soạn tin $\rightarrow$ Gửi $\rightarrow$ Phân loại phản hồi).<br>2. Baseline tốn thời gian lớn nhất (120 phút/ngày).<br>3. Tác động trực tiếp tới doanh thu dịch vụ bảo dưỡng của đại lý. | Khách hàng nhắn lại bằng câu văn không chuẩn (ngôn ngữ tự nhiên) thì AI có nhận diện đúng lịch hẹn không. |
| **Candidate 6: Kiểm tra checklist an toàn cáp treo hằng tuần** | 1. Quy trình kiểm tra cố định, tính chuẩn hóa cao.<br>2. Có bằng chứng pain thực tế từ kỹ sư vận hành cáp treo.<br>3. AI hỗ trợ phát hiện rủi ro bất thường nhanh. | Khó giả lập dữ liệu cảm biến thực tế trong phạm vi buổi lab. |
| **Candidate 2: Trả lời tự động giá phụ tùng & phí bảo dưỡng qua Zalo OA** | 1. Tần suất câu hỏi lặp lại rất cao (85 tin/tuần).<br>2. Đo lường được ngay thời gian phản hồi khách hàng.<br>3. Dữ liệu bảng giá Excel có sẵn tại đại lý. | Khách hỏi các đời xe cũ hoặc hư hỏng kết hợp phức tạp thì AI có thể báo sai giá. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Candidate 1 (Nhắc lịch bảo dưỡng VinFast)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **Candidate 6 (Checklist an toàn cáp treo)** | 4 | 4 | 4 | 4 | 2 | 4 | 4 | **26** |
| **Candidate 2 (Trả lời giá phụ tùng Zalo)** | 5 | 4 | 4 | 4 | 5 | 5 | 4 | **31** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Candidate 1: Nhắc lịch bảo dưỡng định kỳ cho khách hàng qua Zalo/SMS bằng AI Workflow tại đại lý VinFast.
```

**Vì sao chọn (4-5 câu):**
Nhóm chọn bài toán này vì có actor cực kỳ rõ ràng (nhân viên CSKH Khánh và khách hàng đi xe VinFast) cùng workflow tuyến tính chuẩn hóa qua 5 bước. Baseline thời gian lặp đi lặp lại rất nặng (120 phút/ngày cho 30 khách) với 15% tỷ lệ nhầm lẫn mốc bảo dưỡng. Bài toán có metric đầu ra sắc nét (giảm xuống 20 phút/ngày, tăng tỷ lệ khách quay lại bảo dưỡng từ 55% lên 75%). Đặc biệt, nhóm sở hữu dữ liệu quy trình thực tế từ đại lý VinFast, giúp bài làm trong lab có tính khả thi và thực chiến 100%.

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**
- **Candidate 6 (Checklist cáp treo):** Bài toán hay về an toàn nhưng khó thu thập dữ liệu cảm biến thực tế trong thời gian lab, khó kiểm chứng phản hồi.
- **Candidate 2 (Trả lời giá phụ tùng Zalo):** Tần suất cao nhưng scope hẹp hơn bài nhắc lịch, giải pháp nghiêng nhiều về Rule-based FAQ hơn là cần sự cá nhân hóa của AI.

**Disagreement (nếu có — ai lo gì, chốt ra sao):**
Vương lo ngại rằng nếu khách hàng nhắn tin lại bằng câu từ tự nhiên (vd: "mai bận rồi tuần sau nhé", "xe này bán rồi") thì hệ thống sẽ không tự đặt được lịch. Khánh và Thắng đã giải thích và chốt phương án: AI chỉ đóng vai trò phân loại Intent (Ý định) và soạn bản nháp, nhân viên CSKH vẫn là người bấm xác nhận cuối cùng (Human Boundary) và gọi lại nếu AI phân loại có độ tin cậy < 85%.

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Interview** | 3 Cố vấn dịch vụ (SA) & 5 Khách hàng đi xe VinFast | *"Nhiều khi tôi đang họp mà CSKH gọi nhắc lịch bảo dưỡng xe VF8 là tôi tắt máy ngay. Nhưng nếu nhắn Zalo kèm mốc km và bảng phí dự kiến thì tôi xem ngay và nhắn lại giờ rảnh."* (Anh Tuấn - Khách hàng VF8) | 1 khách hàng lớn tuổi nói: *"Tôi không dùng Zalo, CSKH cứ gọi điện trực tiếp cho tôi như trước."* | Bổ sung phương án Fallback: Nếu gửi Zalo không thành công hoặc khách thuộc nhóm lớn tuổi, hệ thống tự động chuyển danh sách cho CSKH gọi điện thủ công. |
| **Mini Survey trong lớp** | 8 học viên | 7/8 người xác nhận từng bị trễ mốc bảo dưỡng xe vì quên lịch hoặc cuộc gọi CSKH đến sai thời điểm. | 1 người cho rằng chỉ cần cài app MyVinFast là đủ. | Thu hẹp phạm vi: Tập trung vào khách hàng chưa cài app MyVinFast, chăm sóc qua kênh Zalo OA phổ thông. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain thật không nằm ở việc khách hàng không muốn bảo dưỡng xe, mà nằm ở việc cuộc gọi nhắc lịch thủ công gây phiền phức sai thời điểm, trong khi tin nhắn SMS thông thường lại quá generic (thiếu mốc km và báo giá dự kiến).
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Zalo ZNS (Zalo Notification Service)** | https://zalo.me/business/zns | Gửi tin nhắn thông báo tự động theo số điện thoại | Tỷ lệ mở tin > 85%, chi phí thấp, gửi đúng Zalo khách | Chỉ gửi được mẫu tin cố định (template), không tự động cá nhân hóa nội dung linh hoạt theo văn cảnh | Dùng ZNS làm kênh hạ tầng gửi tin, kết hợp AI để sinh nội dung cá nhân hóa trước khi đẩy qua ZNS. |
| **MyVinFast App Notification** | https://vinfastauto.com/vn_vi | Tự động nhắc lịch bảo dưỡng trên ứng dụng di động | Chính hãng VinFast, dữ liệu chuẩn | Tỷ lệ khách hàng tải app và bật notification chỉ đạt ~30% | Cần kênh Zalo OA phổ biến hơn cho 70% khách hàng chưa cài app. |
| **SleekFlow / Respond.io (Omnichannel AI Customer Service)** | https://sleekflow.io/features/zalo | Tự động hóa phản hồi Zalo & phân loại tin nhắn | Tích hợp CRM tốt, phân loại intent tự động | Chi phí bản quyền cao, chưa tối ưu cho quy trình đại lý ô tô/xe điện Việt Nam | Học hỏi pattern: AI draft câu trả lời $\rightarrow$ Nhân viên bấm duyệt (Human-in-the-loop). |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Không nên tự build ứng dụng di động riêng hay dùng Agent tự động 100% gây rủi ro gửi sai thông tin. Giải pháp tối ưu nhất là AI Workflow: Script tự động lọc dữ liệu Excel $\rightarrow$ AI sinh tin nhắn Zalo cá nhân hóa $\rightarrow$ CSKH kiểm tra & duyệt gửi $\rightarrow$ AI phân loại ý định phản hồi của khách hàng để chốt lịch.
```

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.md`

```text
[1 Mở Excel & lọc khách đến hạn: 20' - CSKH] 
→ [2 Tra cứu sổ lịch sử bảo dưỡng: 25' - CSKH] 
→ [3 Soạn tin nhắn Zalo & Gọi điện thủ công: 75' - CSKH] <-- bottleneck
→ [4 Ghi nhận phản hồi vào sổ Excel: 20' - CSKH] 
→ [5 Tổng hợp & chuyển lịch cho Cố vấn dịch vụ: 10' - CSKH]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | CSKH (Khánh) | File Excel danh sách mua xe / bảo dưỡng | Danh sách khách hàng đến hạn 1,6,12 tháng | 20 phút / ngày | Thao tác lọc thủ công dễ bỏ sót |
| 2 | CSKH (Khánh) | Biển số xe / SĐT khách hàng | Thông tin dòng xe, số km cũ, phụ tùng thay lần trước | 25 phút / ngày | Tra cứu từng dòng trên Excel |
| 3 | CSKH (Khánh) | Danh sách cần nhắc | Tin nhắn Zalo gửi đi / Cuộc gọi hoàn thành | **75 phút / ngày** | **Bottleneck chính:** 2.5 phút/khách, dồn 30 khách/ngày, 15% sai mốc |
| 4 | CSKH (Khánh) | Phản hồi của khách (nghe máy / nhắn lại) | Sổ ghi chú trạng thái (Đồng ý/Bận/Đổi giờ) | 20 phút / ngày | Phản hồi rải rác, ghi chép dễ nhầm |
| 5 | CSKH (Khánh) | Sổ ghi chú trạng thái | Danh sách lịch hẹn chuyển cho Cố vấn dịch vụ (SA) | 10 phút / ngày | Handoff thủ công qua giấy/zalo nhóm |

**Bottleneck chính (2-3 câu):**
Bottleneck nằm ở Bước 3 khi nhân viên CSKH phải gõ tin nhắn Zalo hoặc gọi điện thủ công cho từng người trong danh sách 30 khách hàng mỗi ngày (tốn 75 phút). Thao tác lặp đi lặp lại mệt mỏi dẫn đến 15% tỷ lệ gửi nhầm tên xe hoặc nhầm mốc km bảo dưỡng.

### 5.2. Future workflow bản nhóm

```text
[1 Auto-pull data đến hạn từ Excel/CRM: 2' - Rule] 
→ [2 AI sinh nội dung tin nhắn Zalo cá nhân hóa: 1' - AI] 
→ [3 CSKH kiểm tra & duyệt gửi danh sách tin (Boundary): 10' - Human] 
→ [4 AI phân loại phản hồi khách (Đồng ý/Đổi lịch): 5' - AI] 
→ [5 CSKH xác nhận & đồng bộ lịch hẹn cho SA: 2' - Human]

Fallback: Khách không dùng Zalo hoặc AI phân loại intent phản hồi có độ tin cậy < 85% -> Chuyển tự động sang danh sách cho CSKH gọi điện tư vấn trực tiếp.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| **Tổng thời gian** | 120 phút/ngày | **20 phút/ngày** | Bấm giờ từ lúc lọc dữ liệu đến khi chốt lịch |
| **Số bước** | 5 bước | 5 bước | Tối ưu hóa tự động ở các bước trung gian |
| **Số bước thủ công** | 5/5 bước thủ công | **2/5 bước thủ công** | CSKH chỉ duyệt tin nháp và xác nhận lịch hẹn cuối |
| **Bottleneck chính** | Soạn tin & gọi điện (75') | Duyệt tin nháp (10') | Human boundary kiểm soát chất lượng |
| **Risk mới** | Nhầm lẫn thông tin do mệt mỏi | AI sinh sai từ ngữ (hallucination) | Khắc phục 100% nhờ bước CSKH review trước khi gửi |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên CSKH (Khánh) tại đại lý VinFast chịu trách nhiệm nhắc lịch bảo dưỡng định kỳ cho khách hàng mua xe. |
| **Workflow** | Hằng ngày mở Excel lọc danh sách khách hàng đến hạn, tra cứu lịch sử sửa chữa, soạn tin nhắn Zalo/gọi điện từng người, ghi nhận phản hồi và chuyển lịch hẹn cho Cố vấn dịch vụ. |
| **Bottleneck** | Thao tác soạn tin nhắn Zalo và gọi điện thủ công cho 30 khách/ngày mất 75 phút, gây quá tải và 15% tỷ lệ nhầm lẫn mốc bảo dưỡng. |
| **Impact** | Tốn 120 phút/ngày (12 giờ/tuần) cho 1 nhân viên CSKH; tỷ lệ khách quay lại bảo dưỡng định kỳ đúng hạn chỉ đạt 55%. |
| **Success Metric** | Giảm tổng thời gian nhắc lịch từ 120 phút xuống dưới 20 phút/ngày; Tăng tỷ lệ khách phản hồi đặt lịch thành công lên 75%. |
| **Boundary** | AI không tự động gửi tin nhắn nếu chưa được CSKH bấm duyệt; AI không tự ý thay đổi giá phụ tùng hoặc chính sách bảo hành. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field mơ hồ: Success metric "tăng trải nghiệm khách hàng" còn định tính; AI intervention point chưa ghi rõ can thiệp trước/sau bước nào.
- Tôi sửa gì: Đổi metric thành con số định lượng (tổng thời gian < 20 phút/ngày, tỷ lệ đặt lịch đạt 75%); bổ sung cụ thể điểm can thiệp của AI vào v1.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [x] Thấp (quy trình bảo dưỡng theo mốc km có quy định rõ) / [ ] Cao
- Độ phức tạp: [ ] Thấp / [x] Cao (phối hợp nhiều nguồn dữ liệu Excel, Zalo API, phân loại phản hồi)

**Bài toán nhóm nằm ở ô nào:**
```text
Ô "Phức tạp cao - Mơ hồ thấp": Workflow điều phối nhiều bước rõ ràng có AI hỗ trợ ngôn ngữ.
```

**Vì sao (2-3 câu):**
Quy trình nhắc lịch có các mốc km và danh mục bảo dưỡng cố định (mơ hồ thấp), nhưng cần kết nối dữ liệu từ Excel, sinh tin nhắn cá nhân hóa và phân loại tin nhắn phản hồi của khách hàng (phức tạp cao). Do đó, hình thức Workflow là phù hợp nhất.

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Tự động lọc danh sách Excel đến hạn & gửi SMS mẫu cố định | Đủ nếu khách hàng chỉ cần tin nhắn nhắc thô không có thông tin cá nhân | Tin nhắn cứng nhắc, tỷ lệ đọc thấp, không xử lý được khi khách nhắn lại | Chọn cho bước 1 (Auto-pull data Excel) |
| **Workflow** | Script lọc Excel $\rightarrow$ AI sinh tin Zalo cá nhân hóa $\rightarrow$ CSKH duyệt $\rightarrow$ AI phân loại phản hồi $\rightarrow$ CSKH chốt lịch | Hợp lý nhất vì quy trình theo bước tuyến tính cố định, AI hỗ trợ ngôn ngữ & phân loại | AI sinh nhầm từ ngữ $\rightarrow$ Đã có CSKH review duyệt trước khi gửi | **CHỌN CHÍNH** (Cho toàn bộ quy trình) |
| **Agent** | AI Agent tự truy cập Zalo, tự nhắn tin, tự thương lượng giờ hẹn và tự ghi lịch vào CRM | Chỉ cần nếu quy trình thương lượng lịch hẹn quá phức tạp và đa dạng nhánh | Rủi ro hallucination nhắn hớ giá/lịch, mất kiểm soát truyền thông đại lý | Không chọn (Quá nhiều rủi ro) |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không? -> Rule giải được bước lọc dữ liệu, nhưng không giải được bước tạo tin cá nhân hóa và phân loại câu trả lời của khách.
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh? -> Các bước đi theo quy trình tuyến tính 5 bước cố định, chỉ rẽ nhánh nhẹ khi khách từ chối/bận.
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không? -> Không cần Agent tự lập kế hoạch động vì tuyến tính công việc đã rất chuẩn hóa.
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu? -> Nhân viên CSKH phát hiện ngay ở bước duyệt tin nháp (Bước 3) và sửa chỉ trong 5-10 giây.
5. Có hạ được từ Agent → Workflow → Rule không? -> Có thể hạ từ Agent xuống Workflow dễ dàng và đây là lựa chọn an toàn nhất.

**Mức chọn:**
```text
Workflow
```

**Vì sao chọn (3-4 câu):**
Nhóm chọn mức Workflow vì bài toán có các bước thực hiện tuyến tính rất rõ ràng. AI chỉ tham gia hỗ trợ ở 2 bước cần năng lực xử lý ngôn ngữ (sinh tin nhắn cá nhân hóa và phân loại Intent phản hồi), các bước còn lại do Rule và con người đảm nhiệm. Mô hình này vừa tối ưu được 80% thời gian vừa giữ được Human Boundary tuyệt đối an toàn cho đại lý VinFast.

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**
Không thể chỉ dùng Rule đơn thuần vì tin nhắn SMS mẫu cố định có tỷ lệ tương tác rất thấp (chỉ ~10%), đồng thời Rule không thể hiểu và phân loại được các câu trả lời tự nhiên của khách hàng khi họ nhắn lại đổi lịch.

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên CSKH (Khánh) tại đại lý VinFast. |
| **Workflow** | Lọc dữ liệu Excel đến hạn $\rightarrow$ Tạo tin nhắn Zalo cá nhân hóa $\rightarrow$ CSKH review duyệt gửi $\rightarrow$ Phân loại phản hồi khách $\rightarrow$ Đồng bộ lịch hẹn cho Cố vấn dịch vụ. |
| **Bottleneck** | Soạn tin nhắn Zalo và gọi điện thủ công cho 30 khách/ngày tốn 75 phút, 15% nhầm lẫn mốc bảo dưỡng. |
| **Impact** | Tốn 120 phút/ngày (12 giờ/tuần); tỷ lệ khách quay lại bảo dưỡng định kỳ đúng hạn chỉ đạt 55%. |
| **Success Metric** | Giảm tổng thời gian xử lý từ 120 phút xuống **dưới 20 phút/ngày**; Tăng tỷ lệ khách phản hồi đặt lịch thành công lên **75%**; Tỷ lệ tin nhắn chính xác 100%. |
| **Boundary** (làm / không làm) | **Làm:** Sinh tin nhắn nháp cá nhân hóa, phân loại intent phản hồi (Đồng ý/Bận/Hủy). **Không làm:** AI không tự gửi tin khi chưa có lệnh của CSKH, không tự thỏa thuận giảm giá phụ tùng ngoài quy định. |
| **AI intervention point** | Can thiệp sau Bước 1 (dùng AI sinh tin từ data Excel) và sau Bước 3 (dùng AI phân loại tin nhắn phản hồi của khách). |
| **Mức chọn** | **Workflow:** Vì quy trình tuyến tính cố định, AI hỗ trợ xử lý ngôn ngữ ở bước cụ thể, có người thật duyệt. |
| **Rủi ro & người thật kiểm tra** | **Rủi ro:** AI hallucination sinh nhầm tên xe hoặc mốc km. **Người kiểm tra:** Nhân viên CSKH kiểm tra danh sách tin nháp ở Bước 3 trước khi bấm nút Gửi hàng loạt. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor Khánh CSKH & 5 bước workflow tuyến tính đã xác định sắc nét. |
| Baseline + metric đo được chưa? | Yes | Baseline 120 phút/ngày và target < 20 phút/ngày hoàn toàn đo được bằng bấm giờ. |
| Data/input đủ dùng chưa? | Yes | File Excel danh sách khách hàng và lịch sử bảo dưỡng có sẵn tại đại lý VinFast. |
| AI sai, hậu quả chấp nhận được không? | Yes | Hậu quả kiểm soát 100% nhờ bước CSKH duyệt tin nháp trước khi gửi out. |
| Có người review/owner không? | Yes | Nhân viên CSKH Khánh trực tiếp làm Owner vận hành hệ thống. |
| Có cách non-AI đơn giản hơn không? | Yes (Nhưng hiệu quả kém) | SMS Marketing mẫu cố định có sẵn nhưng tỷ lệ chuyển đổi kém hơn nhiều so với tin cá nhân hóa AI. |

**Decision:**
```text
Go với scope nhỏ (Pilot).
```

**Lý do (3-4 câu dựa trên bằng chứng):**
Bài toán có pain thật được xác nhận qua phỏng vấn khách hàng, workflow tuyến tính rõ ràng và baseline thời gian đo lường sắc nét (120 phút/ngày). Giải pháp AI Workflow giúp giảm 83% thời gian vận hành mà không phát sinh rủi ro nhờ Human Boundary chặt chẽ. Dữ liệu thực tế tại đại lý VinFast có sẵn, đảm bảo khả năng triển khai thành công cao.

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**
- **Data pilot:** 50 khách hàng đến hạn bảo dưỡng trong 2 tuần tới tại VinFast.
- **Chạy tay:** Lọc Excel $\rightarrow$ Chạy prompt AI tạo 50 tin nháp $\rightarrow$ CSKH review 5 phút $\rightarrow$ Gửi qua Zalo OA $\rightarrow$ Đo phản hồi.
- **3 số đo:** 
  1. Tổng thời gian hoàn thành công việc nhắc lịch (Mục tiêu < 20 phút/ngày).
  2. Tỷ lệ CSKH phải sửa lại tin nháp của AI (Mục tiêu < 10%).
  3. Tỷ lệ khách hàng xác nhận đặt lịch hẹn thành công (Mục tiêu > 70%).

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**
Nếu trong 2 tuần pilot, tỷ lệ tin nhắn nháp AI sinh ra bị sai thông tin phải sửa tay > 40%, hoặc xảy ra 1 sự cố gửi sai mốc bảo dưỡng đến khách hàng, dừng ngay workflow AI và quay về template cố định (Rule-based).

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
��p (chỉ ~10%), đồng thời Rule không thể hiểu và phân loại được các câu trả lời tự nhiên của khách hàng khi họ nhắn lại đổi lịch.

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên CSKH (Khánh) tại đại lý VinFast Hồng Hạnh. |
| **Workflow** | Lọc dữ liệu Excel đến hạn $\rightarrow$ Tạo tin nhắn Zalo cá nhân hóa $\rightarrow$ CSKH review duyệt gửi $\rightarrow$ Phân loại phản hồi khách $\rightarrow$ Đồng bộ lịch hẹn cho Cố vấn dịch vụ. |
| **Bottleneck** | Soạn tin nhắn Zalo và gọi điện thủ công cho 30 khách/ngày tốn 75 phút, 15% nhầm lẫn mốc bảo dưỡng. |
| **Impact** | Tốn 120 phút/ngày (12 giờ/tuần); tỷ lệ khách quay lại bảo dưỡng định kỳ đúng hạn chỉ đạt 55%. |
| **Success Metric** | Giảm tổng thời gian xử lý từ 120 phút xuống **dưới 20 phút/ngày**; Tăng tỷ lệ khách phản hồi đặt lịch thành công lên **75%**; Tỷ lệ tin nhắn chính xác 100%. |
| **Boundary** (làm / không làm) | **Làm:** Sinh tin nhắn nháp cá nhân hóa, phân loại intent phản hồi (Đồng ý/Bận/Hủy). **Không làm:** AI không tự gửi tin khi chưa có lệnh của CSKH, không tự thỏa thuận giảm giá phụ tùng ngoài quy định. |
| **AI intervention point** | Can thiệp sau Bước 1 (dùng AI sinh tin từ data Excel) và sau Bước 3 (dùng AI phân loại tin nhắn phản hồi của khách). |
| **Mức chọn** | **Workflow:** Vì quy trình tuyến tính cố định, AI hỗ trợ xử lý ngôn ngữ ở bước cụ thể, có người thật duyệt. |
| **Rủi ro & người thật kiểm tra** | **Rủi ro:** AI hallucination sinh nhầm tên xe hoặc mốc km. **Người kiểm tra:** Nhân viên CSKH kiểm tra danh sách tin nháp ở Bước 3 trước khi bấm nút Gửi hàng loạt. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor Khánh CSKH & 5 bước workflow tuyến tính đã xác định sắc nét. |
| Baseline + metric đo được chưa? | Yes | Baseline 120 phút/ngày và target < 20 phút/ngày hoàn toàn đo được bằng bấm giờ. |
| Data/input đủ dùng chưa? | Yes | File Excel danh sách khách hàng và lịch sử bảo dưỡng có sẵn tại đại lý VinFast Hồng Hạnh. |
| AI sai, hậu quả chấp nhận được không? | Yes | Hậu quả kiểm soát 100% nhờ bước CSKH duyệt tin nháp trước khi gửi out. |
| Có người review/owner không? | Yes | Nhân viên CSKH Khánh trực tiếp làm Owner vận hành hệ thống. |
| Có cách non-AI đơn giản hơn không? | Yes (Nhưng hiệu quả kém) | SMS Marketing mẫu cố định có sẵn nhưng tỷ lệ chuyển đổi kém hơn nhiều so với tin cá nhân hóa AI. |

**Decision:**
```text
Go với scope nhỏ (Pilot).
```

**Lý do (3-4 câu dựa trên bằng chứng):**
Bài toán có pain thật được xác nhận qua phỏng vấn khách hàng, workflow tuyến tính rõ ràng và baseline thời gian đo lường sắc nét (120 phút/ngày). Giải pháp AI Workflow giúp giảm 83% thời gian vận hành mà không phát sinh rủi ro nhờ Human Boundary chặt chẽ. Dữ liệu thực tế tại đại lý VinFast Hồng Hạnh có sẵn, đảm bảo khả năng triển khai thành công cao.

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**
- **Data pilot:** 50 khách hàng đến hạn bảo dưỡng trong 2 tuần tới tại VinFast Hồng Hạnh.
- **Chạy tay:** Lọc Excel $\rightarrow$ Chạy prompt AI tạo 50 tin nháp $\rightarrow$ CSKH review 5 phút $\rightarrow$ Gửi qua Zalo OA $\rightarrow$ Đo phản hồi.
- **3 số đo:** 
  1. Tổng thời gian hoàn thành công việc nhắc lịch (Mục tiêu < 20 phút/ngày).
  2. Tỷ lệ CSKH phải sửa lại tin nháp của AI (Mục tiêu < 10%).
  3. Tỷ lệ khách hàng xác nhận đặt lịch hẹn thành công (Mục tiêu > 70%).

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**
Nếu trong 2 tuần pilot, tỷ lệ tin nhắn nháp AI sinh ra bị sai thông tin phải sửa tay > 40%, hoặc xảy ra 1 sự cố gửi sai mốc bảo dưỡng đến khách hàng, dừng ngay workflow AI và quay về template cố định (Rule-based).

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do

