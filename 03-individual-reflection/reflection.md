# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Phạm Văn Kiên
- Mã học viên: 2A202602590
- Nhóm: Nhóm Day 02 - AI Product Labs
- Candidate problem nhóm chọn: RoadGuardian - Phát hiện sớm tai nạn giao thông từ camera không được giám sát liên tục

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tôi scan 10 problems quanh bối cảnh sinh viên năm cuối học AI: debug notebook, đọc paper, tổng hợp report, quản lý task nhóm, chuẩn bị CV/portfolio. | Nhóm có thêm nhiều candidate thuộc nhóm học tập/project AI, đặc biệt là các bài có workflow và metric thời gian khá rõ. |
| Pitch Problem Card | Tôi pitch bài "Debug notebook/lab AI" với workflow chạy notebook → gặp log lỗi → đọc log → search/hỏi bạn → sửa → chạy lại. | Bài này được đưa vào danh sách 12 candidates và giúp nhóm có một ví dụ rõ về bottleneck kỹ thuật có thể đo bằng phút/lỗi. |
| Challenge bài của bạn khác | Tôi hỏi lại nhóm với các bài có AI rằng liệu Rule/template/checklist đã đủ chưa, đặc biệt với bài task nhóm, unit test và RoadGuardian. | Nhóm không chọn Agent ngay mà buộc phải nói rõ AI can thiệp ở bước nào, ai review, fallback khi AI sai là gì. |
| Gom trùng / cluster | Tôi hỗ trợ gom 12 candidates thành 4 cụm: developer workflow, học tập/project, RAG/evaluation và RoadGuardian/giao thông thông minh. | Việc cluster giúp nhóm nhìn ra các bài trùng pattern và không bị lẫn giữa problem chính với sub-problem. |
| Chọn candidate problem | Tôi đồng ý đưa RoadGuardian của Đàm Việt Hưng vào shortlist và so sánh với bài unit test boilerplate và RAG error triage. | Nhóm chọn RoadGuardian làm candidate cuối vì impact xã hội cao hơn, workflow rõ và có thể đặt metric như detection latency, recall, false alert rate. |
| Validation / research | Tôi góp ý rằng nhóm chưa nên claim Go vì chưa có interview/log thật; cần ghi rõ validation quote còn thiếu và chỉ coi số liệu hiện tại là giả thuyết. | Bản nhóm giữ decision ở mức Not Yet thay vì khẳng định AI chắc chắn cần triển khai. |
| Workflow nhóm | Tôi góp phần tách current workflow của RoadGuardian thành các bước: tai nạn xảy ra, camera ghi hình, chờ người phát hiện, tiếp nhận, xác minh, xác định vị trí, chuyển thông tin. | Bottleneck được làm rõ ở đoạn camera đã ghi được sự kiện nhưng người có trách nhiệm chưa biết để review. |
| Problem Statement | Tôi rà lại các field actor, bottleneck, impact, success metric và boundary để tránh viết quá rộng kiểu "AI xử lý tai nạn". | Problem Statement tập trung vào phát hiện suspected incident, không tự kết luận pháp lý hay tự điều động lực lượng. |
| Rule / Workflow / Agent | Tôi ủng hộ chọn Workflow, trong đó Rule là baseline và AI chỉ hỗ trợ phát hiện nghi ngờ từ video được cấp quyền. | Nhóm tránh chọn Agent vì bài toán chưa cần AI tự lập kế hoạch hay tự ra quyết định; human verification vẫn là boundary bắt buộc. |
| Decision | Tôi đồng thuận quyết định Not Yet: làm pilot offline nhỏ trước, đo detection latency, recall, false alert rate và human verification time. | Decision có lý do dựa trên thiếu baseline, thiếu dữ liệu camera được cấp quyền và rủi ro privacy/alert fatigue. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là phần ép nhóm nhìn bài toán theo workflow và metric thay vì chọn AI vì nghe hấp dẫn. Tôi cũng góp phần giữ decision ở mức Not Yet, vì RoadGuardian có impact lớn nhưng chưa đủ bằng chứng để khẳng định Go.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Tôi dùng AI để gợi ý thêm problem theo 4 lăng kính sau khi đã tự chọn bối cảnh sinh viên năm cuối học AI. | AI giúp tôi nhớ thêm các pain như debug notebook, tổng hợp kết quả model, quản lý task nhóm và CV/portfolio. | Một số ý quá rộng như "trợ lý AI toàn năng" hoặc "AI tự làm toàn bộ đồ án" không có workflow và boundary rõ. | Tôi giữ lại các pain có dấu hiệu đo được bằng phút/lần, lần/tuần hoặc số tin nhắn hỏi lại; bỏ các ý không phải trải nghiệm thật. |
| Problem Card | Tôi dùng AI để phản biện card debug notebook/lab AI. | AI nhắc tôi làm rõ actor, bottleneck, metric và không để AI tự sửa code. | AI có xu hướng đề xuất workflow hơi rộng, dễ biến thành tool debug tự động quá mức. | Tôi giới hạn lại: AI chỉ đọc log và gợi ý thứ tự kiểm tra, còn sinh viên tự sửa và chạy lại. |
| Workflow | Tôi dùng AI để hỗ trợ sắp xếp current/future workflow thành các bước dễ đọc. | AI giúp biến mô tả rời rạc thành flow có bottleneck, human boundary và fallback. | Nếu để AI tự viết, một số bước bị gom quá nhanh, làm mất chỗ nghẽn thật. | Tôi tách lại các bước như đọc log, search, sửa, chạy lại; với RoadGuardian thì tách rõ camera ghi hình và người phát hiện. |
| Research | Tôi dùng AI/search để gợi ý hướng research cho bài RoadGuardian và nhắc các nguồn cần kiểm chứng. | AI giúp nhắc rằng cần phân biệt context tai nạn giao thông với bằng chứng trực tiếp về workflow camera. | AI có thể đưa số liệu hoặc claim chưa kiểm được, không đủ dùng làm evidence chính. | Tôi chỉ giữ các ý có thể gắn với nguồn hoặc dùng như giả thuyết; phần validation thật vẫn ghi là chưa có quote/log. |
| Problem Statement | Tôi dùng AI để rà xem field nào còn mơ hồ. | AI chỉ ra metric, boundary và baseline là ba điểm dễ yếu. | AI có thể viết lại quá trơn tru khiến nghe như đã validate xong. | Tôi giữ ngôn ngữ thận trọng: prototype target, cần validate, chưa có baseline production. |
| Rule / Workflow / Agent | Tôi dùng AI để so sánh mức Rule, Workflow và Agent. | AI giúp liệt kê rủi ro của Agent: quá nhiều quyền, khó kiểm soát, dễ vượt boundary. | Nếu prompt không chặt, AI thường đẩy bài toán lên Agent cho "xịn" hơn. | Tôi chọn Workflow: Rule làm baseline, AI tạo suspected incident, human review là bắt buộc. |
| Decision | Tôi dùng AI để kiểm tra logic Go/Not Yet/No-Go. | AI giúp nhắc các điều kiện trước khi Go: data, consent, operator review, false alert tolerance. | AI không có dữ liệu thực tế của nhóm nên không thể quyết định thay. | Tôi đồng ý với decision Not Yet và ghi rõ cần phỏng vấn/khảo sát, dataset có quyền và pilot offline trước. |

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
Khi nghe top 3 problems của các bạn khác, tôi nhận ra một problem tốt không nhất thiết phải là problem nghe "AI" nhất, mà là problem có actor, workflow và bottleneck đủ rõ để tranh luận. Ban đầu tôi nghiêng về các bài gần với trải nghiệm của mình hơn như debug notebook hoặc quản lý task nhóm, vì các bài đó dễ đo và dễ validate trong lớp. Tuy nhiên, khi nghe Đàm Việt Hưng pitch RoadGuardian, tôi thấy bài này có khoảng nghẽn rất rõ: camera có thể đã ghi được tai nạn nhưng người có trách nhiệm chưa chắc biết ngay để kiểm tra. Nhóm có lúc hơi dễ bị kéo sang hướng solution-first, kiểu nghĩ ngay đến computer vision phát hiện tai nạn, nhưng sau đó cả nhóm kéo lại bằng câu hỏi AI can thiệp đúng bước nào và con người kiểm tra ở đâu.

Tôi có thay đổi ý kiến sau khi bị challenge vì bài RoadGuardian tuy khó hơn nhưng có impact xã hội rõ hơn các bài developer workflow. Đóng góp thật sự của tôi là giúp nhóm so sánh các candidate bằng workflow, metric và boundary, không chỉ chọn bài vì nghe hay. Tôi cũng góp phần giữ decision ở mức Not Yet, vì nhóm chưa có baseline detection latency, chưa có quote interview và chưa có dữ liệu camera được cấp quyền. Điều khó nhất khi viết Problem Statement là boundary: nếu không cẩn thận, bài này rất dễ trượt từ "phát hiện suspected incident" sang "AI tự xử lý tai nạn", điều đó quá rủi ro. Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở phần validation: phải hỏi ít nhất 2-3 người có liên quan đến camera/tiếp nhận sự cố trước khi viết target metric. Tôi cũng sẽ chuẩn bị trước một bảng so sánh Rule vs Workflow vs Agent để cả nhóm thấy rõ vì sao Workflow hợp lý hơn Agent trong bài này.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
