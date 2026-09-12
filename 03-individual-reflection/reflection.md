# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Thiều Quang Vinh
- Mã học viên: 2A202602877
- Nhóm: Zone A - 6ae
- Candidate problem nhóm chọn: Sinh viên năm 4 làm đồ án / khóa luận mất ~145 phút mỗi lượt để đọc một paper tiếng Anh 25-35 trang trước buổi họp tiến độ (2 lượt/tuần), phần lớn thời gian nằm ở bước đọc kỹ + tra thuật ngữ chuyên ngành rồi tự viết note.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tìm vấn đề từ công việc thực tế của một thực tập sinh và làm đồ án (đọc báo cáo khoa học, viết báo cáo kỹ thuật,...). | Đóng góp 3 bài toán tốn nhiều thời gian nhất từ khi còn đi thực tập vào danh sách chung của nhóm |
| Pitch Problem Card | Trình bày bài toán: "Soạn thảo báo cáo kỹ thuật cho cả lập trình viên lẫn đối tác kinh doanh", phân tích điểm nghẽn khi phải chuyển đổi và dung hợp văn phong giữa hai nhóm người đọc. | Đây là vấn đề có thật, nhưng đối tượng hướng đến hơi lệch so với bối cảnh sinh viên năm 4 làm đồ án của các thành viên còn lại. |
| Challenge bài của bạn khác | Phản biện bài toán Chỉnh CV + cover letter riêng cho từng JD thực tập: Hầu hết chuẩn format của Cover letter đều sử dụng LaTeX và các cấu trúc LLM có thể chỉnh sửa được. Vậy nên, không cần một ứng dụng AI riêng dành cho việc đó  | Nhóm đồng ý để loại bỏ ra khỏi danh sách candidate problem. |
| Gom trùng / cluster | Cùng nhóm tạo ra 6 categories để phân loại 18 bài toán của 6 thành viên; xếp bài báo cáo kỹ thuật vào cụm Viết tài liệu (D), bài phân tích log lỗi vào cụm Truy vết (E), bài rà soát PR vào cụm Cảnh báo sớm (F). | Nhóm đã đồng tinh và chia ra được 6 nhóm. |
| Chọn candidate problem | Phản biện và bảo vệ quan điểm cho các bài toán liên quan đến việc làm doanh nghiệp hơn vì mang tính thực tế hơn để trang bị kiến thức cho việc đi làm. | Chia cuộc phản biện ra thành: 1 bên ủng hộ việc đi theo bài toán kỹ thuật khi đi làm, 1 bên ủng hộ việc chỉ nên giới hạn trong vấn đề của sinh viên. |
| Validation / research | Tìm hiểu các công cụ đọc tài liệu khoa học (SciSpace, Elicit, Zotero) và chỉ ra điểm yếu kỹ thuật: các tệp PDF bài báo thường có cấu trúc 2 cột, chứa nhiều công thức toán và bảng biểu phức tạp nên các công cụ này rất dễ trích xuất sai. | Gợi ý cho nhóm về rủi ro "AI trích xuất sai công thức và số liệu thực nghiệm" vào bảng phân tích giải pháp. |
| Workflow nhóm | Góp ý xây dựng quy trình: Cần kiểm tra các kí hiệu toán học và thuật ngữ chuyên ngành | Đặt ra boundary để user không phụ thuộc hoàn toàn vào LLM |
| Problem Statement | Chuẩn hoá ranh giới vận hành: quy định rõ AI chỉ được giải thích thuật ngữ trong đúng ngữ cảnh bài báo, tuyệt đối cấm tự suy diễn khi chưa đọc hết báo. | Tạo guardrails để LLM không tạo sinh không có chứng cứ ở bước giải thích quan trọng khi đọc hiểu bài báo. |
| Rule / Workflow / Agent | Đề xuất ý kiến xây dựng fully autonomous agent vì các bài toán cần dùng đến thuật ngữ chuyên ngành thì có thể sử dụng guardrails để kiểm soát | Nhóm bác bỏ, thống nhất chọn mức Workflow vì giúp giảm thiểu chi phí gọi mô hình và tránh được rủi ro vòng lặp vô tận. |
| Decision | Cùng nhóm bỏ phiếu chốt quyết định Go ở phạm vi thử nghiệm hẹp. | Quyết định đi tiếp dựa trên số liệu đo lường thực tế. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Đưa ra và bảo vệ ý kiến về việc hướng đến bài toán dành cho người đi làm hơn là sinh viên. Gợi ý và tạo ra phản biện về những cơ hội và rủi ro khi ứng dụng mô hình autonomous agent cho research agent.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Prompt gợi ý 15 problems theo 4 lenses. | Brainstorm nhanh mấy task lặp lại: review PR, check CI/CD log, sinh mock test data. | 1 vài bài toán đưa ra bị hẹp có thể giải quyết chỉ bằng 1-2 rules | Chọn ra những task cần con người review và tìm hiểu lâu và ngốn thời gian nhất. |
| Problem Card | Phản biện với AI để chọn ra 3 bài toán tốt nhất. | Chỉ ra lỗ hổng bài technical report: thiếu business input thì LLM sẽ chém gió sai về cost và ROI. | Trả lời dài lê thê, văn phong marketing sáo rỗng. | Cắt hết chữ thừa, viết lại workflow gãy gọn và gắn fallback rõ ràng khi model hallucinate. |
| Workflow | Sinh sơ đồ ASCII Workflow để hỗ trợ cho team. | Dựng layout nhanh, ước lượng thời gian hoàn thành mỗi module. | Vỡ layout, tổ chức module không đúng | Prompt để đưa ra instruction để nhờ agent sửa lại rồi đưa ra cho các thành viên review. |
| Research | Tìm tài liệu về cách con người làm research | Tổng hợp các bài báo, blog hướng dẫn làm research chung. | Chưa thực sự phân tích được từng bước làm research và cung cấp tài liệu dựa trên đó. | Tìm hiểu về phương pháp NCKH và nhờ các bạn tìm hiểu về cách tự động hoá cho từng bước research. |
| Problem Statement | Gọt lại câu chữ theo format chuẩn 6 fields. | Ráp câu gọn gàng giữa Actor, Bottleneck và Impact. | Phần boundary viết chung chung, thiên về AI Ethics hơn guardrails. | Viết lại boundary thành guardrails kỹ thuật: cấm LLM tự suy diễn khi thiếu context, cấm bịa kết quả thực nghiệm. |
| Rule / Workflow / Agent | Hỏi so sánh trade-off giữa Rule, Workflow và Agent cho bài đọc paper. | Phân tích được sự khác biệt về latency, cost gọi API và độ phức tạp implement. | AI thiên về hướng autonomous agent vì đó là công nghệ mới. | Ban đầu đồng tình, sau khi được team phản biện thì có tìm hiểu lại và chốt việc chỉ sử dụng Workflow. |
| Decision | Không dùng. | Không dùng. | Không dùng. | Việc phân tích kết quả cuối không mất quá nhiều thời gian và dựa trên majority vote. Các thành viên cũng đã bàn bạc đầy đủ trong suốt quá trình. |

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
Mình thay đổi ý kiến khá rõ ở khâu chọn mức độ giải pháp giữa Agent và Workflow. Ban đầu mình cảm thấy có tiềm năng để kiểm soát và khuyên nhóm làm fully autonomous agent, vì nghĩ mấy bài toán đọc paper học thuật chỉ cần set guardrail chặt là agent tự xoay sở được. Nhưng sau khi bị cả team phản biện về rủi ro chi phí, latency cao và nguy cơ agent bị kẹt trong infinite loop khi duyệt mấy file PDF dài, mình đã ngồi research lại và đồng ý lùi về làm Workflow cho an toàn. Với mình, phần khó nhất khi chốt Problem Statement là boundary chứ không hẳn là metric. Metric thời gian hay số lượt đọc thì tụi mình bấm giờ và ước lượng tương đối dễ, nhưng boundary thì rất khó vì AI không hình dung được những việc nào cần sự kiểm soát tuyệt đối từ con người. Vì vậy nên phải bóc tách boundary thành các guardrail kỹ thuật cụ thể: cấm LLM tự suy diễn số liệu khi thiếu context, và bắt buộc user phải tự review các công thức toán cùng bảng biểu thực nghiệm. Nếu có cơ hội làm lại buổi lab này, mình sẽ challenge team mạnh hơn ở bước validation và kiểm thửu giải pháp trên paper thật. Nhóm mình vẫn hơi vội khi chỉ dừng lại ở việc đọc tài liệu hướng dẫn research chung chung và khảo sát bằng miệng. Có thể kiểm chứng bằng các ứng dụng đã build sẵn như Scispace, Perplexity...
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
