# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Trần Cao Thắng
- Mã học viên: 2A202602520
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Sinh viên năm cuối chuyên ngành Kỹ thuật Phần mềm (Software Engineering) kiêm Junior Fullstack Developer / Intern tại một công ty công nghệ phát triển ứng dụng Web SaaS.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Nhận ticket từ Jira backlog, code tính năng (feature) và sửa lỗi (bugfix) trong sprint 2 tuần.
  - Tạo Pull Request (PR), tự kiểm tra code và tham gia peer review PR cho các thành viên khác trong nhóm dự án.
  - Đọc tài liệu API spec (Swagger/OpenAPI), viết unit test và chuẩn bị mock data kiểm thử.
  - Tái hiện lỗi từ bug report của QA/Tester, đọc file log/Sentry để điều tra nguyên nhân gốc rễ (root cause).
  - Họp Daily Scrum hằng sáng và viết cập nhật tiến độ công việc trong sprint.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Tốn thời gian | Đọc hiểu và review Pull Request (PR) lớn (>300 dòng diff) khi thiếu context mô tả chi tiết từ người tạo PR. | Reviewer (Dev), Author PR, Tech Lead | Bấm giờ 5 PR tuần trước: mất 45-60 phút/PR; trung bình 4 PR/tuần; PR bị ngâm (pending review) trung bình 1.5 ngày do reviewer ngại đọc diff dài; quote từ Senior: "Nhìn PR 15 file đổi không biết bắt đầu từ đâu để test logic". |
| 2 | Lặp lại | Viết mock data và fixtures cho Unit Test từ API schema / JSON contract mới. | Developer viết test, QA | Mất 25-30 phút/endpoint; lặp lại 4-6 lần/sprint; phải copy-paste JSON thủ công rồi sửa từng trường ID, email, timestamp, status. |
| 3 | Pain từ người khác | QA/Tester tạo bug ticket thiếu thông tin cụ thể (thiếu payload gọi lỗi, thiếu browser/version, log mơ hồ) khiến Dev phải hỏi đi hỏi lại. | Developer sửa bug, QA | Thống kê 8/10 bug ticket tuần qua phải ping Slack hỏi lại: "Lỗi này test ở account nào?", mất thêm 15-20 phút chờ phản hồi cho mỗi ticket trước khi bắt đầu fix. |
| 4 | Tốn thời gian | Phân tích file log và stack trace lỗi dài hàng trăm dòng từ Sentry / CloudWatch để khoanh vùng hàm nội 
bộ gây crash. | On-call Dev, Backend Dev | Mất 30-40 phút mỗi lần điều tra log; gặp 3 lần/tuần; log bị ngập bởi stack trace của 3rd-party node_modules/framework gây nhiễu, khó định vị dòng code lỗi của team. |
| 5 | Lặp lại | Tổng hợp danh sách commits và PRs đã merge để viết Release Notes / Changelog trước ngày deploy staging/production. | Release Lead, Dev | Mất 40 phút mỗi cuối sprint (2 tuần/lần); phải mở từng PR trên GitHub copy title, đối chiếu ticket Jira để phân loại New Feature / Bug Fix / Breaking Change. |
| 6 | AI có thể tốt hơn | Đọc hiểu và tra cứu các hàm legacy code phức tạp (>200 dòng, không có docstring/comment, người viết cũ đã nghỉ). | Junior Dev, Newcomer | Mất 1.5 - 2 tiếng/lần để vẽ lại luồng chạy; xảy ra 2 lần/tuần; phải chèn console.log/debugger thủ công để hiểu luồng dữ liệu truyền qua các component. |
| 7 | Lặp lại | Viết báo cáo cập nhật Daily Standup mỗi sáng (hôm qua làm gì, hôm nay làm gì, blocker gì) dựa trên commit Git và Jira status. | Cả team Dev (6 người) | Bấm giờ mất 10-15 phút/người mỗi sáng trước 9h15; phải lội lại Git log và Jira board để nhớ hôm qua đã làm những gì; tổng team mất ~1 giờ/ngày cho việc này. |
| 8 | AI có thể tốt hơn | Nghĩ ra các test cases biên (edge cases: giá trị rỗng, số âm, vượt độ dài, phân quyền trái phép) khi viết unit/integration test. | Developer, QA | 3 bug lọt lên môi trường Staging tuần trước đều do bỏ sót trường hợp boundary mà dev không lường trước khi code logic. |
| 9 | Pain từ người khác | Frontend Dev bị block tiến độ, phải chờ Backend Dev hoàn thiện và deploy xong API mock mới ghép được giao diện. | Frontend Dev, PM | Bị block trung bình 1-2 ngày làm việc giữa sprint; Frontend phải tự hardcode dữ liệu giả trong code giao diện, sau đó mất thêm 30 phút dọn dẹp khi nối API thật. |
| 10 | Tốn thời gian | Bóc tách tài liệu đặc tả yêu cầu (SRS/PRD) dài 20-30 trang của khách hàng thành danh sách Jira user stories và tasks kỹ thuật. | Tech Lead, Dev | Mất 3-4 tiếng mỗi buổi Sprint Planning; các quy tắc nghiệp vụ rải rác ở nhiều mục khác nhau, dễ bị sót acceptance criteria quan trọng. |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: *"Tôi là Junior Software Engineer làm việc trong sprint Agile 2 tuần. Hãy liệt kê các tác vụ lặp đi lặp lại và tốn thời gian nhất trong quy trình làm việc hằng ngày của một lập trình viên."*
- Ý dùng được: AI gợi ý góc nhìn về việc đọc file log phân tán (Sentry/CloudWatch) và việc viết changelog/release notes từ Git commits.
- Ý bỏ vì không phải pain thật: AI gợi ý *"Tự động sinh 100% mã nguồn từ yêu cầu khách hàng"* và *"Tự động trả lời email khách hàng"*. Tôi bỏ vì đây là kỳ vọng phi thực tế, rủi ro cao, và Junior Dev không trực tiếp giao tiếp email với khách hàng ngoài dự án.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể (đã làm 10 dòng chi tiết để đạt điểm thưởng bonus).
- [x] Dùng ít nhất 3/4 lăng kính (đủ cả 4 lăng kính: Lặp lại, Tốn thời gian, AI có thể tốt hơn, Pain từ người khác).
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian" (toàn bộ đều có số phút bấm giờ, tần suất lần/tuần, số lượng bug/PR cụ thể).

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đọc hiểu và review Pull Request (PR) lớn (>300 dòng diff) khi thiếu context mô tả chi tiết từ người tạo PR. | 1. Workflow rõ ràng (từ mở PR đến approve/merge).<br>2. Bottleneck cực nặng ở bước reviewer đọc diff code.<br>3. Đo lường chính xác bằng thời gian review và thời gian PR bị treo (pending). | Làm sao lọc bớt các file cấu hình tự sinh (như package-lock.json, build output) để LLM không bị quá tải context và giữ an toàn dữ liệu mã nguồn nội bộ. |
| 2 | QA/Tester tạo bug ticket thiếu thông tin cụ thể (payload, log, account test) khiến Dev phải hỏi đi hỏi lại. | 1. Nỗi đau hai chiều rất lớn giữa Dev và QA.<br>2. Input là text log/mô tả có thể cấu trúc hóa.<br>3. Giảm trực tiếp số tin nhắn ping-pong qua lại trên Slack. | Format log lỗi giữa các service backend và frontend khác nhau; nhiều lỗi phụ thuộc thao tác chuột/UI khó mô tả chỉ bằng text. |
| 3 | Viết mock data và fixtures cho Unit Test từ API schema / JSON contract mới. | 1. Tần suất lặp lại cao (mỗi khi có API mới).<br>2. Input là OpenAPI/Swagger schema có cấu trúc rất chặt chẽ.<br>3. Rút ngắn thời gian dev viết test. | Đã có nhiều công cụ Rule-based sinh mock data (như Faker, Prism), cần làm rõ AI vượt trội ở điểm nào (ví dụ: tạo dữ liệu có tính logic nghiệp vụ và test case biên). |

---

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Chuẩn bị context & draft checklist review Pull Request (PR Review Assist)

```text
Problem 1 câu:
Khi nhận Pull Request lớn (>300 dòng code), Reviewer mất 45-60 phút để đọc diff và mường tượng luồng chạy do PR description sơ sài, dẫn đến việc PR bị treo trung bình 1.5 ngày và review dễ sót lỗi logic nghiệp vụ.

Actor:
Reviewer (Junior/Senior Software Engineer) và Author (người tạo PR).

Thời điểm / bối cảnh:
Sau khi Developer hoàn thành code tính năng và mở Pull Request trên GitHub/GitLab trước khi merge vào nhánh chính (develop/main).

Current workflow 3-7 bước:
1. Author tạo PR, điền mô tả sơ sài ("fix bug", "add feature X") rồi gán Reviewer. (2')
2. Reviewer nhận thông báo, mở PR trên GitHub, đọc tiêu đề và mô tả. (3')
3. Reviewer mở tab "Files changed", cuộn qua lại giữa 10-15 file diff, tự suy luận luồng dữ liệu thay đổi. (30') <-- Bottleneck chính
4. Reviewer mở Jira ticket đọc lại Acceptance Criteria để so sánh xem code có đáp ứng đúng yêu cầu không. (10')
5. Reviewer viết comment góp ý hoặc yêu cầu sửa đổi, hoặc nhấn Approve nếu thấy ổn. (10')
6. Author đọc comment, sửa code nếu có, sau đó Reviewer duyệt lại và Merge. (5')

Bottleneck:
Bước 3 (Đọc và đối chiếu 300+ dòng diff qua nhiều file): Mất 30 phút vì reviewer phải tự đọc chay từng dòng thay đổi mà không có bản đồ tóm tắt (change summary) phân nhóm theo chức năng và rủi ro tiềm ẩn.

Impact:
- Mỗi reviewer mất 45-60 phút/PR, với 4 PR/tuần tốn 3-4 tiếng/tuần/người.
- Cả team 6 người tốn ~20 giờ/tuần.
- PR bị treo 1.5 ngày làm chậm chu kỳ phát hành sprint (lead time increase).
- Do mệt mỏi khi đọc diff dài, reviewer hay "LGTM" (Looks Good To Me) lướt qua, làm lọt 2-3 bug logic lên Staging mỗi tháng.

Success metric:
- Giảm thời gian review trung bình từ 60 phút xuống dưới 20 phút/PR.
- Giảm thời gian chờ PR (PR turnaround time) từ 36 giờ xuống dưới 8 giờ.
- Không làm tăng số bug hồi quy (regression bugs) lọt lên Staging.

Non-AI alternative:
1. Ép quy định PR Template bắt buộc tác giả viết đủ 5 mục (Context, Changes, How to test, Risk, Screenshot).
2. Dùng GitHub Action chia nhỏ PR (cảnh báo nếu diff > 300 lines).
3. Linter/SonarQube tự động kiểm tra cú pháp và code smells.
-> Hạn chế: Tác giả thường chống đối hoặc copy paste đối phó vào PR template; Linter chỉ bắt được lỗi cú pháp, không hiểu được business logic xem code có đúng spec Jira không.

AI hypothesis:
Một workflow tự động: Khi PR được tạo, tool tự gom Git Diff và Jira spec -> AI phân tích tóm tắt: (1) Thay đổi chính là gì, (2) Luồng dữ liệu thay đổi ra sao, (3) Gợi ý 3-5 điểm rủi ro/edge cases cần reviewer soi kỹ. Reviewer dựa vào checklist này để review có trọng tâm. Reviewer là người ra quyết định cuối cùng (không cho AI tự merge).

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 60 phút

[1 Author tạo PR: 2'] 
→ [2 Reviewer mở PR: 3'] 
→ [3 Đọc 300+ diff & tự luận luồng: 30']  <-- BOTTLENECK CHÍNH (tốn sức, dễ nản)
→ [4 Mở Jira đối chiếu spec: 10'] 
→ [5 Comment & Approve: 10'] 
→ [6 Merge: 5']

FUTURE STATE — 18 phút

[1 Author tạo PR: 2']
→ [2 Script tự động kéo diff + Jira spec: 1' - Rule]
→ [3 AI tóm tắt logic thay đổi + sinh checklist kiểm tra: 1' - AI]
→ [4 Reviewer đọc tóm tắt & soi code theo checklist định hướng: 12']  <-- HUMAN BOUNDARY (Reviewer thật duyệt)
→ [5 Comment & Approve: 2']
→ [6 Merge code: 1']

Fallback: nếu AI phân tích sai hoặc tóm tắt nhạt nhẽo → Reviewer bỏ qua phần tóm tắt của AI, quay về đọc Git Diff thủ công như cách cũ. Tuyệt đối AI không có quyền tự bấm Approve hoặc Merge code!
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Chuẩn hóa & Phân loại Bug Report từ Staging Log (Bug Triage Assist)

```text
Problem 1 câu:
Khi phát hiện lỗi trên Staging, QA mất nhiều thời gian mô tả thủ công và copy log vụn vặt, khiến Developer mất 30-45 phút điều tra và phải hỏi lại nhiều lần do thiếu các bước tái hiện chuẩn xác.

Actor:
QA/Tester (người báo bug) và Developer (người nhận và sửa bug).

Thời điểm / bối cảnh:
Giai đoạn kiểm thử tính năng trên môi trường Staging/UAT trước khi nghiệm thu release.

Current workflow 3-7 bước:
1. QA gặp lỗi trên UI, chụp ảnh màn hình và mở Console log trình duyệt. (5')
2. QA mở Jira tạo bug ticket, tự gõ tay các bước tái hiện và dán console log. (10')
3. Dev nhận ticket, đọc mô tả nhưng không hiểu ngữ cảnh hoặc thiếu payload API. (5')
4. Dev ping Slack hỏi QA tài khoản test, data mẫu, và yêu cầu QA làm lại để Dev trace log backend. (15') <-- Bottleneck chính
5. Dev mò file log backend theo mốc thời gian, tìm thấy lỗi và xác nhận bug. (10')

Bottleneck:
Bước 4 (Trao đổi qua lại giữa Dev và QA để làm rõ môi trường, tài khoản và payload gây lỗi): Mất 15-20 phút chờ đợi và làm gián đoạn dòng công việc của cả hai bên.

Impact:
- Tốn 45 phút cho mỗi bug được xác nhận. Với 8-10 bug/sprint, tổng thời gian trao đổi lãng phí là 6-8 giờ.
- Gây ức chế tâm lý giữa bộ phận Dev và QA ("Bên này bảo lỗi, bên kia bảo chạy bình thường trên máy tôi").

Success metric:
- Giảm thời gian xác định nguyên nhân và tái hiện bug từ 45 phút xuống dưới 15 phút.
- Giảm số lượng bug ticket phải comment hỏi lại thông tin từ 80% xuống dưới 15%.

Non-AI alternative:
Tạo form Jira bắt buộc (Custom fields: Version, Account Type, Steps to reproduce, Expected, Actual).
-> Hạn chế: QA gõ tay rất tốn thời gian; nhiều khi không biết log backend nằm ở đâu để lấy.

AI hypothesis:
Một extension hoặc bot: QA chỉ cần cung cấp URL lỗi + thao tác + text log thô -> AI tự động phân tích cấu trúc log, trích xuất mã lỗi, URL endpoint, gợi ý 3 bước tái hiện ngắn gọn và gán nhãn độ ưu tiên (Severity).

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 45 phút

[1 QA thấy lỗi: 5'] 
→ [2 QA gõ ticket gõ tay: 10'] 
→ [3 Dev đọc ticket mơ hồ: 5'] 
→ [4 Ping qua lại hỏi account/payload: 15']  <-- BOTTLENECK CHÍNH
→ [5 Dev mò log & xác nhận: 10']

FUTURE STATE — 14 phút

[1 QA copy raw error log & màn hình lỗi: 2'] 
→ [2 AI phân tích trích xuất endpoint, lỗi, tạo form reproduce chuẩn: 1' - AI] 
→ [3 QA rà nhanh 1 phút và submit ticket: 1' - Human boundary] 
→ [4 Dev nhận ticket đầy đủ thông tin, mở đúng file code xử lý: 10']

Fallback: Nếu AI trích xuất sai nguyên nhân → QA tự điền thông tin bổ sung vào Jira ticket như cũ.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Sinh Mock Data & Edge Cases từ OpenAPI Schema (API Mock & Boundary Test)

```text
Problem 1 câu:
Developer mất 25-35 phút để nghĩ và gõ tay các bộ dữ liệu test (cả dữ liệu chuẩn lẫn dữ liệu biên lỗi) cho mỗi endpoint mới, dẫn đến việc test hời hợt và lọt bug validation ra môi trường Staging.

Actor:
Backend Developer (viết Unit Test) và Frontend Developer (cần Mock Data để ghép UI).

Thời điểm / bối cảnh:
Đầu sprint khi Backend mới thiết kế xong file Swagger/OpenAPI spec nhưng chưa code xong logic server, hoặc khi viết test case kiểm thử.

Current workflow 3-7 bước:
1. Dev mở file Swagger/OpenAPI spec để đọc cấu trúc request/response JSON. (5')
2. Dev tạo file mock_data.json trong dự án. (2')
3. Dev tự nghĩ và gõ từng trường dữ liệu mẫu (tên, ngày sinh, tiền tệ, trạng thái enum). (10')
4. Dev cố gắng nghĩ thêm các trường hợp biên: chuỗi rỗng, số âm, ký tự đặc biệt, XSS string để test hàm validate. (15') <-- Bottleneck chính
5. Lưu file và import vào test runner. (3')

Bottleneck:
Bước 4 (Nghĩ và gõ các case dữ liệu biên phức tạp): Mất 15 phút, đòi hỏi trí nhớ và sự cẩn thận. Thường dev chỉ nghĩ được 1-2 case cơ bản rồi bỏ qua vì lười gõ.

Impact:
- Mất 35 phút/endpoint. Team làm 10 endpoint/sprint mất gần 6 tiếng chỉ để gõ dữ liệu giả lập.
- Bỏ sót các lỗi bảo mật và validation dữ liệu (SQL injection mẫu, ký tự unicode tiếng Việt có dấu, ngày tháng sai format).

Success metric:
- Giảm thời gian tạo bộ dữ liệu mock và edge cases từ 35 phút xuống dưới 8 phút.
- Tăng độ bao phủ kiểm thử (Test boundary coverage) thêm ít nhất 4 edge cases/endpoint.

Non-AI alternative:
Dùng thư viện Faker.js hoặc công cụ sinh mock data Prism/Mockaroo tự động từ OpenAPI schema.
-> Hạn chế: Faker.js chỉ sinh dữ liệu ngẫu nhiên vô nghĩa (random string), không hiểu logic quan hệ giữa các trường (ví dụ: ngày kết thúc phải sau ngày bắt đầu, mã bưu chính khớp với thành phố) và không tự tạo các edge cases phá vỡ logic nghiệp vụ.

AI hypothesis:
Đưa OpenAPI YAML schema vào prompt -> AI đọc các validation rule (regex, min, max, enum) -> AI tự động sinh 1 bộ Happy Case + 3 bộ Edge Cases có ngữ cảnh nghiệp vụ thực tế (kèm giải thích tại sao case đó dễ gây crash).

Quick gut:
[ ] No AI / process fix
[x] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 35 phút

[1 Đọc spec: 5'] 
→ [2 Tạo file mock: 2'] 
→ [3 Gõ data mẫu thông thường: 10'] 
→ [4 Nghĩ & gõ edge cases hiểm hóc: 15']  <-- BOTTLENECK CHÍNH
→ [5 Lưu & test: 3']

FUTURE STATE — 8 phút

[1 Đưa Swagger/OpenAPI YAML vào script: 1' - Máy] 
→ [2 Rule check schema format: 1' - Máy] 
→ [3 AI sinh Happy Case + 3 Edge Cases ngữ nghĩa: 2' - AI] 
→ [4 Dev review dữ liệu mẫu và chọn dùng: 3' - Human boundary] 
→ [5 Lưu vào test file: 1']

Fallback: Nếu AI sinh dữ liệu sai type hoặc thiếu trường → Dev dùng Faker.js sinh data ngẫu nhiên chuẩn schema và tự gõ bổ sung edge cases.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Chuẩn bị context & draft checklist review Pull Request (PR Review Assist).
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
1. Workflow rõ ràng và lặp lại liên tục: Mọi thành viên trong nhóm công nghệ đều phải tạo và review PR hằng ngày (3-5 PR/tuần/người).
2. Số đo thời gian và điểm nghẽn cực kỳ chuẩn xác: Giảm thời gian đọc diff từ 30 phút xuống 10 phút, tổng thời gian review từ 60 phút xuống 18 phút/PR, và giảm thời gian treo PR từ 1.5 ngày xuống dưới 8 giờ.
3. Impact to lớn và ranh giới rõ ràng: Giúp team release sprint đúng hạn, chống mệt mỏi cho reviewer, đồng thời có Human Boundary cực kỳ vững chắc (AI chỉ tóm tắt và sinh checklist gợi ý, quyền Approve/Merge 100% thuộc về kỹ sư con người).
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. "Nếu AI tóm tắt diff quá mượt và đưa ra checklist tưởng như đầy đủ, liệu Reviewer có sinh ra tâm lý ỷ lại (automation bias), chỉ lướt qua checklist rồi bấm Approve luôn mà không thèm đọc code thật không? Làm sao để thiết kế workflow buộc reviewer phải thực sự kiểm tra code?"
2. "Việc gửi Git Diff và Jira ticket lên mô hình ngôn ngữ lớn (LLM) có nguy cơ vi phạm bảo mật mã nguồn độc quyền của dự án (IP leak) hay không? Làm sao giải quyết bằng giải pháp kỹ thuật (Self-hosted model / Data sanitization)?"
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: AI ban đầu nhận xét rằng *"Review code là việc trí tuệ cao, tại sao không để một AI Agent tự đọc code, tự chạy test và tự merge code luôn để tiết kiệm 100% thời gian của lập trình viên?"*
- Tôi sửa gì: Tôi nhận ra AI đang bị căn bệnh "Solution-first / Agent-first" cực kỳ nguy hiểm. Giao toàn quyền merge code cho AI sẽ dẫn đến thảm họa bảo mật, phá vỡ kiến trúc hệ thống và hallucination. Tôi đã bác bỏ và sửa lại: AI chỉ dừng lại ở mức **Workflow hỗ trợ (PR Review Assist)** — chuẩn bị bối cảnh và gợi ý checklist rủi ro, con người bắt buộc giữ quyền kiểm soát tại chốt chặn cuối cùng.

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field (Đã scan 10 problems có số đo cụ thể, vượt mức tối thiểu để đạt điểm bonus).
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback.
- [x] Đã chọn 1 card pitch + câu hỏi challenge có chiều sâu phản biện.
