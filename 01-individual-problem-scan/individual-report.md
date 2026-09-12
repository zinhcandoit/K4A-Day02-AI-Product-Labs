# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Thiều Quang Vinh
- Mã học viên: 2A202602877
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): intern AI Engineer
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Nhận yêu cầu tính năng, đọc tài liệu đặc tả (spec) và thiết kế hệ thống
  - Viết mã nguồn (code), viết kiểm thử đơn vị (unit test) và tạo dữ liệu kiểm thử giả lập
  - Mở yêu cầu gộp mã (Pull Request), sửa lỗi khi luồng kiểm thử tự động (CI/CD) báo lỗi
  - Tham gia họp nhóm hàng ngày, viết báo cáo tiến độ và tài liệu kỹ thuật định kỳ cho sếp

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | **Tốn thời gian** | Đọc và chắt lọc methodology / baseline metrics từ 5–10 bài báo khoa học (ArXiv/IEEE) cho môn đồ án/seminar. | Sinh viên làm khóa luận, lab research | Mất **3–4 tiếng/bài báo**; mỗi đợt làm đồ án cần đọc 8–10 bài, hay bị quá tải thông tin và bỏ sót công thức/dataset cốt lõi. |
| 2 | **Pain từ người khác** | Giảng viên/Trợ giảng (TA) liên tục bị sinh viên hỏi trùng các câu hỏi về môi trường cài đặt, deadline, quy định nộp bài. | TA, Giảng viên, Sinh viên lớp đông | TA nhận **20–30 tin nhắn/tuần** trên Zalo/Discord hỏi cùng 1 nội dung quy định bài nộp dù đã pin trên nhóm. |
| 3 | **Tốn thời gian** | Viết Unit Test và Mock Data cho các hàm xử lý logic nghiệp vụ mới. | Backend Dev, Intern Software Engineer | Viết test chiếm **40–50% tổng thời gian code** sprint (khoảng 3–4 tiếng/tuần); dev thường lười viết khiến test coverage dưới 50%. |
| 4 | **Lặp lại** | Đọc log lỗi dài hàng trăm dòng từ server/CI-CD để xác định nguyên nhân gốc (Root Cause Analysis). | Dev, DevOps, Tester | Khi build fail hoặc crash test, mất **20–30 phút/lần** lọc qua stack trace để tìm dòng code gây exception; xảy ra **3–5 lần/ngày**. |
| 5 | **AI có thể tốt hơn** | Viết Release Notes và Changelog từ danh sách git commit / pull request để gửi khách hàng hoặc team lead. | Lead dev, Product Owner | Cuối mỗi sprint mất **60–90 phút** để lọc các commit lặt vặt (fix typo, refactor) thành bản tóm tắt tính năng dễ hiểu cho người ngoài. |
| 6 | **Tốn thời gian** | Tổng hợp biên bản cuộc họp (Meeting Minutes) và trích xuất danh sách Action Items (ai làm gì, deadline khi nào). | Thư ký, PM, các thành viên họp | Sau mỗi cuộc họp 1 tiếng, mất thêm **30–45 phút** để nghe lại ghi âm hoặc đọc note nháp để soạn mail tóm tắt. |
| 7 | **Tốn thời gian + AI có thể tốt hơn** | Soạn thảo báo cáo kỹ thuật đa góc nhìn (Technical Report): vẽ kiến trúc, chuẩn hóa template, điều chỉnh nội dung theo stakeholder (Kinh tế vs Kỹ thuật). | Tech Lead, Dev, Sinh viên làm đồ án | Mất **6–8 tiếng/bản báo cáo** 15–20 trang; phải viết 2 phiên bản riêng cho Sếp/Khách hàng (nhấn mạnh ROI, chi phí) và Dev team (nhấn mạnh schema, architecture). Thường trễ deadline 1–2 ngày. |
| 8 | **Lặp lại** | Pre-review Pull Request (PR): Soi các lỗi cơ bản về coding convention, naming, thiếu validate input, sót config trước khi Senior review logic. | Tech Lead, Senior Dev, Member tạo PR | Mỗi tuần review **15–20 PRs**, mất **15–20 phút/PR** chỉ để comment nhắc các lỗi format/style lặp lại; làm chậm thời gian merge code trung bình thêm **1–2 ngày**. |
| 9 | **Tốn thời gian** | Tạo bộ dữ liệu kiểm thử biên (Synthetic Edge-case Test Data): Giả lập dữ liệu biên, dữ liệu dị biệt (ký tự lạ, số âm, ngày sai định dạng) để test độ bền hệ thống. | QA/Tester, Dev | Viết script tạo mock data tốn **2–3 tiếng/chức năng lớn**; thường chỉ test được luồng chuẩn (happy path), bỏ sót edge case dẫn tới lỗi crash khi demo/production. |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: "Gợi ý thêm các problem trong môi trường lập trình/học tập theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn, pain từ người khác; kèm actor, workflow sơ bộ và số đo thật."
- Ý dùng được: "Ý tưởng về pre-review Pull Request (PR) kiểm tra convention/security và sinh synthetic edge-case data cho testing. Đây là hai nỗi đau thực tế thường gặp khi code dự án."
- Ý bỏ vì không phải pain thật: "Bỏ các ý về chatbot tư vấn kiến trúc tự động hoặc trợ lý toàn năng, vì quá rộng, thiếu khả năng kiểm soát và không phản ánh workflow hàng ngày."

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | **#7: Soạn thảo báo cáo kỹ thuật cho nhiều đối tượng: Cấp quản lý/Kinh doanh (tiến độ, chi phí, rủi ro) và Đội ngũ lập trình (kiến trúc, API)** | • Quy trình rõ ràng: Đi từ ghi chú kỹ thuật thô đến 2 bản tài liệu riêng biệt cho Quản lý và Lập trình viên.<br>• Điểm nghẽn lớn: Kỹ sư mới mất 4–5 tiếng chuyển ngữ cảnh từ kỹ thuật sang kinh doanh, thường bị trả về sửa 2–3 lần.<br>• Đo lường được: Giảm từ 430 phút xuống dưới 90 phút. | AI dễ viết chung chung hoặc suy đoán sai số liệu kinh tế nếu tài liệu kỹ thuật đầu vào thiếu thông tin nghiệp vụ. |
| 2 | **#4: Đọc và phân tích nhật ký lỗi (log) khi luồng kiểm thử tự động (CI/CD) hoặc máy chủ gặp sự cố** | • Quy trình chuẩn xác: Xảy ra ngay khi luồng kiểm thử tự động thất bại, từ lúc tải nhật ký lỗi đến khi tìm ra dòng mã gây lỗi.<br>• Điểm nghẽn rõ ràng: Mất 20–30 phút lọc hàng trăm dòng thông báo rác của thư viện để tìm vết lỗi (stack trace).<br>• Phân định rõ tầng xử lý: Dùng Rule lọc rác, dùng AI giải thích nguyên nhân và cách sửa. | Tệp nhật ký quá dài vượt giới hạn ngữ cảnh của mô hình hoặc vô tình chứa thông tin bảo mật (mã truy cập, mật khẩu). |
| 3 | **#8: Rà soát sơ bộ yêu cầu gộp mã (Pre-review Pull Request): Quét lỗi đặt tên, quy chuẩn lập trình và kiểm tra biên** | • Tác động thực tế: Giảm 15–20 phút/lần duyệt cho kỹ sư chính, giảm 1–2 ngày chờ đợi sửa lỗi vặt cho kỹ sư mới.<br>• Quy trình tích hợp sẵn: Chạy trực tiếp trên tiến trình tự động hóa mã nguồn (GitHub Actions / GitLab CI).<br>• Kết hợp bổ trợ: Bộ kiểm tra cú pháp tĩnh (Linter) bắt lỗi quy tắc, mô hình ngôn ngữ bắt lỗi ngữ nghĩa và thiếu sót kiểm tra biên. | Mô hình có thể đưa ra cảnh báo sai hoặc máy móc với các đoạn mã đặc thù của dự án, gây phiền cho lập trình viên. |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Soạn thảo Báo cáo Kỹ thuật Đa Góc nhìn (Technical Report theo Stakeholder)

```text
Problem 1 câu:
Người viết báo cáo kỹ thuật mất 6–8 tiếng để chuẩn hóa tài liệu và phải viết lại nhiều lần vì không điều chỉnh được góc nhìn phù hợp giữa đối tượng Kinh tế (Sếp/Khách hàng cần ROI, chi phí) và Kỹ thuật (Dev team cần schema, kiến trúc, API).

Actor:
Tech Lead, Senior Developer, hoặc Sinh viên làm đồ án tốt nghiệp / đồ án môn học.

Thời điểm / bối cảnh:
Cuối mỗi đợt phát triển tính năng (sprint) hoặc khi bàn giao giai đoạn (milestone), cần nộp báo cáo đồng thời cho Quản lý dự án (cần tiến độ, chi phí, rủi ro) và Đội ngũ lập trình (cần kiến trúc, lược đồ dữ liệu, API).

Current workflow 3-7 bước:
1. Thu thập dữ liệu kỹ thuật: mã nguồn đã làm, tài liệu thiết kế, số liệu đo hiệu năng (45').
2. Mở khung mẫu báo cáo chuẩn của công ty (30').
3. Vẽ sơ đồ kiến trúc hệ thống và luồng dữ liệu (60').
4. [BOTTLENECK] Viết nội dung chi tiết và chuyển đổi giọng văn cho 2 đối tượng: bản cho Quản lý (chi phí, tiến độ, rủi ro) và bản cho Lập trình viên (kiến trúc, lược đồ dữ liệu, API) (240').
5. Đọc rà soát, căn chỉnh định dạng và kiểm tra tính nhất quán (45').
6. Xuất tệp tài liệu và gửi cho các bên liên quan (10').

Bottleneck:
Bước 4 — Việc chuyển đổi cách diễn đạt từ chi tiết kỹ thuật chuyên sâu sang ngôn ngữ kinh doanh tốn tới 240 phút (hơn 55% tổng thời gian) và thường bị quản lý yêu cầu viết lại vì quá nhiều thuật ngữ khó hiểu.

Impact:
Mất 430 phút (~7.2 tiếng) cho mỗi bản báo cáo (ước tính từ 2 lần viết gần nhất gồm cả thời gian sửa); 30–40% báo cáo bị trả về sửa 2–3 lần; trễ hạn nộp tài liệu 1–2 ngày, ảnh hưởng đến tiến độ phê duyệt tính năng.

Success metric:
- Giảm tổng thời gian hoàn thành báo cáo từ 430 phút xuống dưới 90 phút.
- Số lần bị quản lý yêu cầu viết lại do lệch góc nhìn/giọng văn giảm từ 2–3 lần xuống 0 lần.
- 100% sơ đồ và bảng số liệu tuân thủ đúng khung mẫu chuẩn của công ty.

Non-AI alternative:
Dùng template có sẵn kèm khung câu hỏi gợi ý để kỹ sư tự điền. Cách này chỉ chuẩn hóa được hình thức, không giúp kỹ sư mới tự động chuyển đổi từ dữ liệu kỹ thuật sang ngôn ngữ kinh doanh.

AI hypothesis:
LLM đóng vai trò Semantic Adapter: Nhận đầu vào là tài liệu thiết kế kỹ thuật + số liệu thô + mục tiêu kinh doanh, sau đó tự sinh 2 bản tóm tắt phù hợp với từng stakeholder (Executive Summary nhấn mạnh ROI/chi phí cho Sếp; Technical Specification nhấn mạnh kiến trúc/API cho Dev). Người viết chỉ cần rà soát và tinh chỉnh.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 430 phút

[1 Thu thập dữ liệu: 45'] → [2 Tạo khung theo mẫu: 30'] → [3 Vẽ sơ đồ kiến trúc: 60'] → [4 Viết nội dung theo 2 góc nhìn: 240']  <-- điểm nghẽn → [5 Rà soát & định dạng: 45'] → [6 Xuất bản & gửi: 10']

FUTURE STATE — 75 phút

[1 Thu thập dữ liệu: 30'] → [2 Tạo khung mẫu tự động & vẽ sơ đồ: 5'] → [3 AI sinh 2 bản thảo theo đối tượng: 5'] → [4 Kỹ sư kiểm tra, xác thực số liệu & tinh chỉnh: 30']  <-- ranh giới người duyệt → [5 Xuất bản & gửi: 5']

Fallback: nếu AI sinh nội dung sai thuật ngữ hoặc suy đoán sai số liệu kinh tế, kỹ sư quay về dùng khung mẫu chuẩn và tự viết tay phần diễn giải.
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Phân tích Log Lỗi CI/CD & Server (Root Cause Analysis)

```text
Problem 1 câu:
Kỹ sư phần mềm mới mất 20–30 phút mỗi khi luồng kiểm thử tự động (CI/CD) báo lỗi hoặc máy chủ gặp sự cố chỉ để dò trong hàng trăm dòng thông báo lỗi (stack trace) nhằm tìm ra dòng mã gây lỗi và nguyên nhân thực sự.

Actor:
Backend Developer, DevOps Engineer, Tester.

Thời điểm / bối cảnh:
Khi đẩy mã nguồn lên hệ thống kiểm thử tự động (CI/CD) bị báo lỗi (build/test thất bại), hoặc khi máy chủ môi trường chạy thử trả về mã lỗi 500.

Current workflow 3-7 bước:
1. Nhận thông báo kiểm thử / triển khai thất bại qua tin nhắn nội bộ (2').
2. Mở bảng điều khiển CI/CD, tải tệp nhật ký thô dài 500–1000 dòng (3').
3. [BOTTLENECK] Dò qua hàng trăm dòng cảnh báo thừa của thư viện, tìm vết lỗi thực sự và suy luận nguyên nhân gốc (20').
4. Mở công cụ lập trình (IDE), tìm đúng tệp và dòng mã được chỉ định (5').
5. Sửa lỗi logic hoặc cấu hình, đóng gói và đẩy lại mã lên hệ thống (10').

Bottleneck:
Bước 3 — Nhật ký kiểm thử quá dài, lẫn lộn giữa cảnh báo thông thường và lỗi nghiêm trọng; kỹ sư mới thiếu kinh nghiệm mất nhiều thời gian để bóc tách đâu là nguyên nhân gốc và đâu là lỗi dây chuyền kéo theo.

Impact:
Mất 20–30 phút cho mỗi lần dò lỗi; xảy ra 3–5 lần/ngày đối với một kỹ sư mới (tổng cộng 1.5–2 tiếng/ngày). Làm tắc nghẽn tiến độ ghép mã và chậm nhịp phát hành của toàn đội.

Success metric:
- Thời gian trích xuất nguyên nhân gốc và dòng mã lỗi giảm từ 20 phút xuống dưới 2 phút.
- Tỷ lệ chỉ ra chính xác dòng mã nguồn và nguyên nhân gây lỗi ngay lần đầu đạt trên 90%.

Non-AI alternative:
Dùng câu lệnh lọc văn bản (grep / biểu thức chính quy) để tìm các từ khóa ERROR, FATAL, Exception. Cách này lọc bớt dòng rác nhưng không giải thích được các lỗi logic phức tạp (xung đột phiên bản thư viện, thiếu biến môi trường, xung đột bất đồng bộ).

AI hypothesis:
Quy trình kết hợp Luật và Trí tuệ nhân tạo: Dùng biểu thức chính quy (Rule) cắt bỏ 80% nhật ký rác của hệ điều hành và thư viện, sau đó gửi đoạn báo lỗi cốt lõi kèm đoạn mã nguồn liên quan cho mô hình ngôn ngữ để tóm tắt nguyên nhân gốc bằng tiếng Việt và gợi ý hướng xử lý. Kỹ sư tự kiểm tra lại và sửa mã.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 40 phút

[1 Nhận thông báo lỗi: 2'] → [2 Mở nhật ký thô: 3'] → [3 Đọc vết lỗi & tìm nguyên nhân: 20']  <-- điểm nghẽn → [4 Tra cứu mã nguồn: 5'] → [5 Sửa & đẩy mã: 10']

FUTURE STATE — 18 phút

[1 Nhận thông báo lỗi: 2'] → [2 Lọc sạch nhật ký rác bằng biểu thức chính quy: 0.5'] → [3 AI tóm tắt lỗi & chỉ dòng mã nghi vấn: 0.5'] → [4 Kỹ sư kiểm tra & xác nhận nguyên nhân: 5']  <-- ranh giới người duyệt → [5 Sửa mã & đẩy lại: 10']

Fallback: nếu AI chẩn đoán sai nguyên nhân, kỹ sư mở tệp nhật ký thô ban đầu và tự tra cứu thủ công theo cách truyền thống.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Rà Soát Sơ Bộ Yêu Cầu Gộp Mã (Pre-review Pull Request: Quy Chuẩn Lập Trình & Kiểm Tra Biên)

```text
Problem 1 câu:
Tech Lead / Senior Dev mất 15–20 phút cho mỗi Pull Request (PR) chỉ để comment nhắc nhở các lỗi lặp lại về naming, coding convention, thiếu validate input và sót config, khiến thời gian duyệt PR bị kéo dài thêm 1–2 ngày.

Actor:
Tech Lead, Senior Developer (Reviewer) và Developer tạo PR.

Thời điểm / bối cảnh:
Mỗi khi lập trình viên hoàn thành một tính năng hoặc sửa lỗi, gửi yêu cầu gộp mã (Pull Request - PR) lên hệ thống quản lý mã nguồn (GitHub / GitLab) để xin gộp vào nhánh chính.

Current workflow 3-7 bước:
1. Kỹ sư mới mở yêu cầu gộp mã với 5–15 tệp thay đổi (5').
2. [BOTTLENECK] Kỹ sư chính mở phần mã thay đổi (git diff), đọc từng dòng để bắt các lỗi: đặt tên sai quy ước, định dạng không đồng nhất, thiếu kiểm tra giá trị rỗng/biên, sót cấu hình nhạy cảm (20').
3. Kỹ sư chính viết bình luận yêu cầu chỉnh sửa (5').
4. Kỹ sư mới đọc phản hồi, sửa lại mã nguồn và đẩy lên (thời gian chờ đợi qua lại mất 12–24 tiếng).
5. Kỹ sư chính kiểm tra lại các điểm đã sửa, sau đó mới tập trung đánh giá logic kiến trúc sâu (10').
6. Phê duyệt và gộp mã vào nhánh chính (2').

Bottleneck:
Bước 2 — Kỹ sư chính tốn thời gian và năng lượng cho các lỗi hình thức, cú pháp bề mặt thay vì tập trung vào kiến trúc hệ thống và logic nghiệp vụ; kỹ sư mới phải chờ đợi phản hồi nhiều vòng.

Impact:
Tiêu tốn 15–20 phút/PR của nhân sự chủ chốt (4–6 tiếng/tuần với 15–20 PRs); yêu cầu gộp mã bị kéo dài thêm 1–2 ngày chỉ vì sửa các lỗi quy ước lặt vặt.

Success metric:
- Giảm 80% số lượng bình luận thủ công về lỗi quy ước đặt tên, định dạng và thiếu kiểm tra dữ liệu cơ bản.
- Thời gian chu chuyển của yêu cầu gộp mã (từ lúc tạo đến khi được gộp) giảm từ 48 tiếng xuống dưới 12 tiếng.

Non-AI alternative:
Cài đặt công cụ kiểm tra tĩnh (Linter: ESLint, Prettier, SonarQube) vào quy trình tự động. Cách này bắt triệt để lỗi cú pháp và thụt lề, nhưng không hiểu được ngữ nghĩa (tên biến có sát nghiệp vụ không, có bỏ sót trường hợp biên đặc thù của chức năng không).

AI hypothesis:
Quy trình kết hợp: Sau khi công cụ kiểm tra cú pháp chạy xong, tích hợp mô hình ngôn ngữ vào tiến trình CI để đọc phần mã thay đổi (git diff), đối chiếu với tài liệu quy ước của nhóm nhằm tự động bình luận nhắc nhở cho kỹ sư mới sửa trước. Kỹ sư chính chỉ cần tập trung đánh giá kiến trúc và logic nghiệp vụ.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 42 phút (chưa tính thời gian chờ đợi phản hồi 24 tiếng)

[1 Mở PR: 5'] → [2 Đọc mã soi lỗi quy ước/đặt tên/kiểm tra rỗng: 20']  <-- điểm nghẽn → [3 Nhắn yêu cầu sửa: 5'] → [4 Đọc lại & đánh giá logic sâu: 10'] → [5 Gộp mã: 2']

FUTURE STATE — 18 phút (cắt giảm các vòng chờ đợi phản hồi lặp lại)

[1 Mở PR: 5'] → [2 Công cụ kiểm tra tĩnh + AI quét mã thay đổi & bình luận tự động: 1'] → [3 Kỹ sư mới tự sửa trước khi thông báo kỹ sư chính: 5'] → [4 Kỹ sư chính chỉ tập trung đánh giá kiến trúc: 6']  <-- ranh giới người duyệt → [5 Phê duyệt & gộp mã: 1']

Fallback: nếu AI bình luận sai hoặc cảnh báo không cần thiết, kỹ sư có thể bỏ qua bình luận đó. Kỹ sư chính vẫn là người giữ quyền quyết định cuối cùng trước khi bấm gộp mã.
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Soạn Thảo Báo Cáo Kỹ Thuật Cho Nhiều Đối Tượng (Cấp Quản Lý & Đội Ngũ Lập Trình)
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Workflow viết báo cáo kỹ thuật là một pain point có thật và lặp lại đối với mọi kỹ sư, dev và sinh viên làm đồ án; trong đó bước chuyển đổi góc nhìn từ kỹ thuật sang kinh tế/nghiệp vụ tốn đến 4–5 tiếng và thường xuyên bị từ chối/bắt sửa lại. Việc áp dụng AI giúp rút ngắn thời gian từ 430 phút xuống dưới 90 phút, đồng thời chuẩn hóa template và sơ đồ kiến trúc cho toàn bộ dự án. Đây là bài toán mà vai trò của LLM thể hiện rõ nét nhất (chuyển dịch ngữ cảnh) mà các công cụ Rule-based thông thường hoàn toàn bó tay.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Làm thế nào để ngăn AI "tự bịa" số liệu kinh doanh (tiến độ, chi phí hạ tầng) khi tài liệu kỹ thuật thô ban đầu không có đủ dữ liệu tài chính?
2. Đâu là ranh giới bắt buộc kỹ sư phải tự tay kiểm tra và chịu trách nhiệm trước khi gửi báo cáo cho cấp quản lý?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: "Nếu chỉ cung cấp tài liệu kỹ thuật mà không có mục tiêu kinh doanh cụ thể, AI sẽ sinh ra nội dung chung chung, sáo rỗng hoặc tự suy đoán sai lệch về mặt chi phí."
- Tôi sửa gì: "Bổ sung quy định đầu vào bắt buộc phải có cả 2 phần (Đặc tả kỹ thuật + Mục tiêu kinh doanh từ cấp quản lý), đồng thời đặt ranh giới người duyệt bắt buộc phải đối chiếu và xác nhận số liệu tài chính trước khi xuất bản."

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
