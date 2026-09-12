# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Trần Cao Thắng
- Mã học viên: 2A202602520
- Nhóm: Nhóm VinFast CSKH (Nguyễn Duy Khánh, Nguyễn Triệu Vững, Trần Cao Thắng)
- Candidate problem nhóm chọn: Tự động hóa quy trình tra cứu danh sách, tạo tin nhắn Zalo cá nhân hóa và phân loại phản hồi nhắc lịch bảo dưỡng định kỳ cho đại lý VinFast bằng AI Workflow.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Quét 10 bài toán thực tế thuộc 4 lăng kính, đưa ra 3 bài toán của bản thân vào danh sách nhóm (Sentiment review, Đối chiếu hợp đồng, Phân loại ticket IT). | Đóng góp Candidate 7, 8, 9 vào bảng tổng hợp ý tưởng của nhóm, giúp nhóm có góc nhìn đa dạng từ vận hành đến kỹ thuật. |
| Pitch Problem Card | Pitch bài toán phân loại và gán priority cho ticket IT Helpdesk, trình bày rõ bottleneck ở bước đọc text phân loại và metric trễ KPI. | Nhóm hiểu rõ cách xác định bottleneck định lượng và cách đo lường thời gian xử lý ticket. |
| Challenge bài của bạn khác | Challenge bài giám sát hồ bơi & checklist cáp treo của Vững về việc đòi hỏi thiết bị camera/cảm biến đắt đỏ khó pilot; challenge bài VinFast của Khánh về việc khách nhắn lại bằng từ ngữ tự nhiên thì hệ thống xử lý thế nào. | Vững đồng ý chuyển sang bài toán có tính khả thi cao hơn; Khánh bổ sung cơ chế AI phân loại Intent phản hồi có ngưỡng tin cậy < 85%. |
| Gom trùng / cluster | Cùng nhóm gom 9 candidate thành 3 cụm A, B, C; chỉ ra mẫu số chung của Cụm A là "Chăm sóc & Nhắc lịch dịch vụ theo quy trình tuyến tính". | Nhóm định hình rõ ràng cụm bài toán có workflow rõ nhất để đưa vào vòng đánh giá shortlist. |
| Chọn candidate problem | Chấm điểm ma trận 7 tiêu chí, ủng hộ bài toán nhắc lịch bảo dưỡng VinFast của Khánh (35 điểm) thay vì bài của bản thân. | Nhóm đạt đồng thuận 100% chọn bài toán VinFast vì có dữ liệu thực tế tại xưởng và baseline đo lường được ngay. |
| Validation / research | Đảm nhiệm vai trò **Research Specialist**: trực tiếp tra cứu và phân tích 3 giải pháp thực tế (Zalo ZNS, MyVinFast App, SleekFlow) kèm link chính thức. | Giúp nhóm nhận ra không cần tự xây dựng hệ thống từ đầu mà chỉ cần kết hợp hạ tầng ZNS với AI sinh nội dung cá nhân hóa. |
| Workflow nhóm | Cùng Vững và Khánh chuẩn hóa 5 bước workflow hiện trạng (nghẽn 75 phút) và tương lai (20 phút); trực tiếp đề xuất cơ chế Fallback (nếu khách không dùng Zalo hoặc AI phân loại intent < 85% thì chuyển CSKH gọi điện). | Quy trình của nhóm trở nên chặt chẽ, có đường lui rõ ràng, đảm bảo không bỏ sót bất kỳ khách hàng nào. |
| Problem Statement | Phản biện bản draft v0 của nhóm; yêu cầu sửa lại Success Metric từ chung chung ("tăng trải nghiệm") thành định lượng cụ thể (< 20 phút/ngày, tỷ lệ đặt lịch 75%). | Problem Statement v1 đạt chuẩn sắc nét, có boundary rõ ràng (làm gì và tuyệt đối không làm gì). |
| Rule / Workflow / Agent | Trực tiếp lập luận và bảo vệ phương án chọn **Workflow**; kiên quyết phản đối ý định làm "Autonomous Agent tự động chat và chốt lịch". | Ngăn chặn được rủi ro AI hallucination báo sai giá phụ tùng hoặc lịch bảo dưỡng, bảo vệ uy tín đại lý VinFast. |
| Decision | Cùng nhóm thống nhất quyết định **Go (Pilot nhỏ)**; xây dựng kịch bản thử nghiệm trên 50 khách hàng trong 2 tuần và điều kiện rollback nếu lỗi > 40%. | Bản quyết định cuối cùng có cơ sở thực chứng vững chắc, khả thi để áp dụng thực tế ngay trong tuần tới. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là phần Research giải pháp (Phase 4.2) với các đường link và bài học đối chiếu thực tế từ Zalo ZNS / SleekFlow, cùng việc thiết lập Human Boundary và cơ chế Fallback ở Phase 5 & 6 để kiềm chế nhóm không sa đà vào làm Agent tự động hoàn toàn gây rủi ro cho đại lý.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm các đầu mục công việc hay lặp lại trong môi trường kỹ thuật và vận hành. | Giúp mở rộng góc nhìn sang các tác vụ phân tích log và phân loại ticket phân tán. | AI gợi ý các ý tưởng viển vông như "Tự động sinh 100% code từ yêu cầu" hoặc "Tự trả lời email khách hàng". | Tôi chủ động gạt bỏ các ý tưởng thiếu kiểm soát, chỉ giữ lại các bài toán có quy trình lặp lại thực tế và có người chịu trách nhiệm rõ ràng. |
| Problem Card | Nhờ AI phản biện và tìm điểm yếu trong các bước workflow của Problem Card #1. | Chỉ ra reviewer thường nản nhất khi phải cuộn qua lại giữa nhiều file diff không có tóm tắt. | AI đề xuất cho bot tự động Approve và Merge code luôn nếu test pass để tiết kiệm 100% thời gian. | Tôi nhận định điều này cực kỳ nguy hiểm và sửa lại thành: AI chỉ đóng vai trò tóm tắt và sinh checklist gợi ý, quyền Approve/Merge 100% thuộc về con người. |
| Workflow | Gợi ý cách phân tách các bước theo mô hình Rule / AI / Human trên Mermaid. | Giúp biểu diễn luồng dữ liệu trực quan và phân định rõ bước nào máy làm, bước nào người làm. | AI gộp bước CSKH duyệt tin và bước gửi tin qua Zalo thành một bước tự động hoàn toàn. | Tôi tách riêng bước CSKH review thành một nút Human Boundary bắt buộc để nhân viên kiểm tra thông tin xe trước khi gửi ra ngoài. |
| Research | Tìm kiếm các nền tảng tự động hóa CSKH qua Zalo và ứng dụng nhắc lịch xe. | Gợi ý nhanh các công cụ như Zalo ZNS, SleekFlow, Respond.io để nhóm tìm hiểu. | AI trích dẫn các con số thống kê tỷ lệ mở tin nhắn 95% nhưng không có link nguồn chính thức để kiểm chứng. | Tôi tự truy cập trang chủ chính thức của Zalo Business và SleekFlow để lấy link xác thực và đọc đúng tài liệu kỹ thuật của họ. |
| Problem Statement | Nhờ AI đóng vai Mentor khó tính để soi các điểm mơ hồ trong Problem Statement v0. | Phát hiện ra trường Success Metric của nhóm ban đầu còn nặng tính định tính ("khách hài lòng hơn"). | AI viết phần Boundary quá rộng, ôm đồm thêm cả tính năng thanh toán trực tuyến và đặt cọc phụ tùng. | Tôi rút gọn Boundary về đúng phạm vi lõi của lab: chỉ hỗ trợ tạo tin nhắn nháp cá nhân hóa và phân loại phản hồi, tuyệt đối không can thiệp giá bán. |
| Rule / Workflow / Agent | Yêu cầu AI so sánh ưu nhược điểm của Rule-based SMS với AI Voice Agent tự gọi điện. | Phân tích rõ chi phí rẻ của Rule và khả năng thấu hiểu ngữ cảnh của AI. | AI liên tục khuyên nên xây dựng "Autonomous Voice Agent tự gọi điện chốt lịch cho ngầu và tối tân". | Tôi phân tích cho nhóm thấy rủi ro pháp lý, chi phí API cuộc gọi thoại quá đắt và nguy cơ khách hàng bực mình khi nghe bot nói chuyện; kiên quyết chọn giải pháp Workflow qua Zalo. |
| Decision | Gợi ý các chỉ số đánh giá thành công khi chạy thử nghiệm (pilot metrics). | Gợi ý chỉ số tỷ lệ nhân viên phải sửa tay tin nhắn nháp (edit rate) rất hay và thực tế. | AI đề xuất thời gian chạy thử nghiệm quá dài (3-6 tháng) trên toàn bộ tệp khách hàng của showroom. | Tôi thu hẹp quy mô pilot xuống 50 khách hàng trong 2 tuần tại một xưởng dịch vụ duy nhất để đo lường nhanh và có đường lui (exit/rollback) an toàn. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Quá trình làm việc cùng nhóm ở Day 02 Lab đã mang lại cho tôi một góc nhìn hoàn toàn mới về tư duy giải quyết vấn đề bằng công nghệ: bài toán tốt không phải là bài toán nghe có vẻ "AI" nhất, mà là bài toán có nỗi đau thực tế và quy trình đo lường được. Ban đầu, khi nghe Khánh trình bày về việc nhân viên CSKH tại đại lý VinFast phải mất 2 tiếng mỗi ngày để gõ tay từng tin nhắn nhắc lịch bảo dưỡng, tôi đã lập tức bị thuyết phục vì đây là một workflow tuyến tính có số liệu quá rõ ràng. Tuy nhiên, nhóm tôi cũng từng có thời điểm bị cuốn vào tâm lý "solution-first", khi cả nhóm hào hứng bàn về việc tạo ra một AI Agent tự động gọi điện hoặc tự chat qua lại để chốt lịch hẹn với khách hàng cho "ngầu". Ở thời điểm đó, tôi đã đóng vai trò là người kéo nhóm về mặt đất khi chỉ ra rủi ro AI có thể hallucination báo sai giá phụ tùng hoặc bịa đặt mốc bảo dưỡng, làm tổn hại nghiêm trọng đến hình ảnh chuyên nghiệp của hãng xe. Đóng góp rõ nét nhất của tôi trong bản báo cáo cuối cùng chính là phần Research giải pháp thực tế đối chiếu với Zalo ZNS và việc thiết lập chốt chặn Human Boundary bắt buộc nhân viên CSKH phải bấm duyệt trước khi tin nhắn được phát đi. Điều tôi thấy khó nhất khi hoàn thiện Problem Statement chính là việc định nghĩa Boundary: phải thực sự can đảm để gạch bỏ những tính năng hấp dẫn nhưng nằm ngoài phạm vi cốt lõi nhằm giữ cho bài toán đủ hẹp và khả thi. Nếu được làm lại từ đầu buổi lab, tôi sẽ challenge nhóm sớm hơn về việc khảo sát thêm nhóm khách hàng lớn tuổi không dùng Zalo ngay từ Phase 4, để kịch bản xử lý cuộc gọi dự phòng (Fallback) được thiết kế mượt mà hơn nữa.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards (Đã làm 10 problems chi tiết, có số liệu đo lường).
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1).
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài (Phase 3 trong group-report.md đầy đủ cluster, shortlist, score).
- [x] [15đ] Nhóm có workflow trước/sau (Phase 5 có đủ 5 bước trước/sau, chỉ rõ bottleneck 75' và boundary).
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ (v1 có đủ 9 trường chi tiết).
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent (Bảng so sánh chi tiết, bảo vệ vững chắc lựa chọn Workflow).
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ (Quyết định Go kèm kế hoạch pilot 50 khách trong 2 tuần).
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì.
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI.
