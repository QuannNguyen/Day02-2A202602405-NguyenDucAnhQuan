# 02 - Group Problem Statement (Bản nộp nhóm)

> Bản tổng hợp từ `individual-report.md` và `indiviual_report2.md`. `individual-report3.md` hiện đang rỗng, vì vậy các candidate cá nhân của ba thành viên bổ sung chưa được điền giả.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|---|---|---|---|
| 1 | Dương Đức Vương | 2A202602944 | Facilitator, validation |
| 2 | Nguyễn Đức Anh Quân | 2A202602405 | Workflow, research |
| 3 | Đỗ Hoàng Quân | 2A202603016 | Domain, AI prototype |
| 4 | Nguyễn Ngọc Linh | 2A202602480 | Research, validation |
| 5 | Lê Thị Trâm Anh | 2A202602846 | Writer, documentation |

**Phân công bổ sung:** Dương Đức Vương phụ trách điều phối và validation; Nguyễn Ngọc Linh phụ trách research và thu thập dữ liệu; Lê Thị Trâm Anh phụ trách viết và chuẩn hóa báo cáo.

**Candidate problem nhóm chọn (1 câu):**

Nhân viên vận hành phải đọc, phân loại và chuyển tiếp thông tin không có cấu trúc từ nhiều nguồn; một workflow AI có human review có thể tạo bản tóm tắt/JSON để giảm thời gian xử lý mà vẫn giữ quyền quyết định cho người phụ trách.

---

## Phase 3 - Group Convergence

### 3.1. Top candidates từ các báo cáo đã nhận

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Nguyễn Đức Anh Quân | Tổng hợp task/deadline từ Discord, Zalo, Google Docs | Leader và thành viên nhóm | Đọc, đối chiếu và gom thông tin từ nhiều kênh | Workflow rõ, nhưng cần giới hạn phạm vi nguồn |
| 2 | Nguyễn Đức Anh Quân | Tìm lại tài liệu, quyết định và file cũ trước deadline | Cả nhóm | Search và xác định đúng phiên bản | Pain lặp lại, cần kho dữ liệu có quyền truy cập |
| 3 | Nguyễn Đức Anh Quân | Viết báo cáo/README từ nhiều nguồn rời rạc | Người viết báo cáo | Đọc, tóm tắt, tạo draft và sửa format | AI phù hợp ở bước outline/draft, không nên tự viết toàn bộ |
| 4 | Đỗ Hoàng Quân | Xử lý sự cố pin xe Xanh SM và điều phối xe sạc/cứu hộ | Dispatcher và tài xế | Đối chiếu GPS, trạm sạc, % pin và soạn hướng dẫn | Impact lớn, nhưng rủi ro vận hành và dữ liệu realtime cao |
| 5 | Đỗ Hoàng Quân | Phân loại và định tuyến ticket cư dân Vinhomes | CSKH và cư dân | Đọc ticket không cấu trúc, chọn danh mục và BQL | Workflow rõ, lặp lại cao, đo được tốt |
| 6 | Đỗ Hoàng Quân | Chẩn đoán sơ bộ lỗi xe VinFast từ mô tả tiếng Việt | Kỹ thuật viên và khách hàng | Hỏi lại triệu chứng và tra cứu tài liệu | AI hiểu ngôn ngữ tự nhiên, nhưng risk sai chẩn đoán cao |
| 7 | Đỗ Hoàng Quân | Tổng hợp lý do khách hủy cuốc từ ghi âm và ghi chú | BA/Ops | Nghe mẫu và tìm pattern thủ công | Có thể mở rộng nhưng cần dữ liệu ghi âm |
| 8 | Đỗ Hoàng Quân | Trích xuất release notes từ commit/PR | Kỹ sư, QA và Ops | Hiểu commit viết tắt và chuyển thành nội dung để test | Phạm vi nhỏ, dễ làm prototype |
| 9 | Dương Đức Vương, Nguyễn Ngọc Linh, Lê Thị Trâm Anh | Chưa có candidate từ báo cáo cá nhân | Chưa xác định | Chưa xác định | Cần bổ sung các báo cáo cá nhân |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A - Tổng hợp tri thức nhóm | 1, 2, 3 | Thông tin rời rạc, người dùng phải đọc và chuyển thành bản có cấu trúc | Phù hợp workflow AI có review |
| B - Triage và routing vận hành | 4, 5, 6 | Đầu vào tự nhiên/nhiều hệ thống, cần phân loại và chọn hành động tiếp theo | Cần boundary và fallback chặt |
| C - Tóm tắt vận hành | 7, 8 | Chuyển ghi âm, commit hoặc log thành summary cho người khác xử lý | Dễ prototype nếu có dữ liệu mẫu |
| D | 9 | Chưa có thông tin | Chờ bổ sung report 3 |

### 3.3. Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| Phân loại và định tuyến ticket cư dân Vinhomes | 200 ticket/ngày theo báo cáo; workflow 4 bước; metric thời gian và accuracy rõ | Chưa có tập ticket đã ẩn danh; ticket multi-intent chưa rõ |
| Tổng hợp task/deadline nhiều kênh | Lặp lại 2-3 lần/tuần; pain ảnh hưởng cả nhóm; có human review tự nhiên | Quyền truy cập Discord/Zalo/Docs và nguồn sự thật chưa rõ |
| Xử lý sự cố pin nguy cấp cho Xanh SM | 80-100 vụ/ngày; bottleneck 15 phút; impact doanh thu lớn | Ranh giới an toàn, API realtime và trách nhiệm khi sai cao |

### 3.4. Score để đồng thuận

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Phan loai/routing ticket cu dan | 5 | 5 | 4 | 5 | 4 | 5 | 3 | 31 |
| Tong hop task/deadline nhieu kenh | 5 | 5 | 4 | 4 | 3 | 4 | 4 | 29 |
| Xu ly su co pin nguy cap | 5 | 5 | 4 | 5 | 2 | 3 | 3 | 27 |

**Candidate nhóm chọn:**

```text
Hỗ trợ phân loại và định tuyến ticket phản ánh cư dân bằng AI, với CSKH review trước khi chuyển đến BQL phù hợp.
```

**Vì sao chọn:**

```text
Candidate có actor, đầu vào, workflow và đầu ra rõ ràng: CSKH nhận ticket, đọc nội dung, phân loại, chọn BQL và chuyển tiếp. Báo cáo cá nhân ước tính khoảng 200 ticket/ngày/khu đô thị và 8 phút/ticket, nên có thể đo baseline bằng thời gian xử lý, accuracy và tỷ lệ route đúng. AI phù hợp để trích xuất entity và tạo JSON, trong khi CSKH vẫn giữ quyền review. Phạm vi prototype có thể giới hạn vào một số danh mục và một khu đô thị.
```

**Vì sao không chọn candidate còn lại:**

```text
Tổng hợp task/deadline từ nhiều kênh có pain rõ nhưng phụ thuộc nhiều nền tảng và quyền truy cập, trong khi nhóm chưa có dữ liệu lịch sử để kiểm chứng. Xử lý sự cố pin có impact lớn nhưng sai sót có thể gây tổn thất vận hành và cần API realtime, vượt quá phạm vi lab hiện tại. Các candidate viết báo cáo, tìm file và release notes dễ prototype nhưng impact nhỏ hơn và chưa được cả nhóm ưu tiên.
```

**Disagreement:**

```text
Nguyễn Đức Anh Quân ưu tiên bài toán tổng hợp task vì gần với workflow học tập; Đỗ Hoàng Quân ưu tiên ticket routing vì có volume và metric rõ hơn. Dương Đức Vương, Nguyễn Ngọc Linh và Lê Thị Trâm Anh tham gia validation, research và chuẩn hóa báo cáo. Nhóm tạm chốt ticket routing theo điểm số và khả năng kiểm thử, nhưng phải xác nhận lại bằng validation và bổ sung các báo cáo cá nhân còn thiếu trước khi Go.
```

---

## Phase 4 - Quick Validation + Research

### 4.1. Quick validation

Chưa có interview/survey độc lập trong ba file đầu vào. Các con số dưới đây là quan sát/ước tính từ cá nhân, không phải quote đã xác minh.

| Nguồn | Số người/mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Báo cáo của Đỗ Hoàng Quân | 1 người quan sát, ước tính 200 ticket/ngày | 8 phút/ticket; CSKH đọc và chọn BQL thủ công | Chưa có log/ticket mẫu | Giữ candidate dạng hypothesis, giới hạn vào ticket một intent |
| Báo cáo của Nguyễn Đức Anh Quân | 1 nhóm học tập, 4 người | Xác nhận pain chung là thông tin rời rạc và cần checklist | Không trực tiếp validate ticket cư dân | Dùng để so sánh, không dùng làm bằng chứng domain Vinhomes |
| Interview/survey người dùng | Chưa thực hiện | Chưa có quote nguyên văn | Chưa có | Cần phỏng vấn 2-3 CSKH/dispatcher hoặc dùng tập ticket ẩn danh |

**Insight sau validation:**

```text
Chưa đủ bằng chứng để kết luận pain 200 ticket/ngày là đại diện cho mọi khu đô thị. Pain cần kiểm chứng là thời gian đọc và route ticket không có cấu trúc; prototype chỉ nên xử lý một số danh mục có quy tắc rõ và luôn để CSKH review.
```

### 4.2. Research giải pháp đã có

| Nguồn/tool/case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống/rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Microsoft Power Automate - AI Builder text classification | [Microsoft Learn](https://learn.microsoft.com/en-us/ai-builder/text-classification-overview) | Phân loại text theo nhãn | Tích hợp workflow và human review | Phụ thuộc dữ liệu huấn luyện, multi-intent khó | Bắt đầu bằng classification có nhãn |
| Azure AI Language - custom text classification | [Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-services/language-service/custom-text-classification/overview) | Gắn nhãn danh mục cho văn bản | Có custom category và API | Cần tập dữ liệu ẩn danh, theo dõi drift | Định nghĩa taxonomy nhỏ và metric F1/accuracy |
| Structured outputs với Azure OpenAI | [Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/structured-outputs) | Trích xuất entity, mức độ khẩn và BQL | JSON dễ kết nối workflow | JSON hợp lệ không đồng nghĩa thông tin đúng | Validate schema, confidence và bước review |

**Research takeaway:**

```text
Nên build workflow nhỏ: nhận ticket -> trích xuất trường có cấu trúc -> gợi ý danh mục/BQL -> CSKH review -> chuyển tiếp. Không nên build agent tự lập kế hoạch, không nên tự động chuyển ticket khi confidence thấp, và không nên đưa ra cam kết SLA khi chưa có dữ liệu thực.
```

---

## Phase 5 - Workflow + Problem Statement

### 5.1. Current workflow

```text
[1 Nhan ticket: 1'] -> [2 Doc va hieu noi dung: 4'] -> [3 Chon danh muc/BQL: 2'] -> [4 Gui xac nhan va chuyen ticket: 1']
```

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|
| 1 | CSKH | Ticket, ảnh, thông tin căn hộ | Ticket được mở | 1 phút, hằng ngày | Nguồn từ App Resident/CRM |
| 2 | CSKH | Mô tả tự nhiên, ảnh đính kèm | Hiểu sơ bộ về vấn đề | 4 phút | Bottleneck; nội dung không cấu trúc |
| 3 | CSKH | Nội dung đã đọc, danh bạ BQL | Danh mục và nơi nhận | 2 phút | Có thể nhầm với ticket multi-intent |
| 4 | CSKH/BQL | Ticket đã phân loại | Ticket được route | 1 phút | Handoff sang BQL |

**Bottleneck chinh:**

```text
CSKH phải đọc và diễn giải lại văn bản tự nhiên trước khi chọn danh mục và BQL. Nếu thiếu thông tin hoặc ticket có nhiều ý, việc route sai làm tăng thời gian phản hồi; AI chỉ nên gợi ý và đánh dấu độ tin cậy, không tự động quyết định mọi trường hợp.
```

### 5.2. Future workflow

```text
[1 Nhan ticket - he thong] -> [2 Rule kiem tra truong bat buoc] -> [3 AI trich xuat JSON va goi y danh muc/BQL] -> [4 CSKH review, sua neu can - boundary] -> [5 He thong chuyen ticket]

Fallback: confidence < 0.85, schema lỗi, ticket multi-intent hoặc AI timeout thì đưa vào hàng đợi xử lý thủ công; không tự động route.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Thời gian xử lý ticket | 8 phút | <= 2 phút | Timestamp nhận đến route |
| Số bước thủ công | 4 | 1-2 | Đếm thao tác của CSKH |
| Accuracy route | Chưa có baseline | >= 92% | So sánh với nhãn đúng do reviewer |
| Ticket bị trả về/sửa route | Chưa có baseline | Giảm 30% | Log route và correction |
| Risk mới | Không áp dụng | AI route sai | Audit mẫu và fallback |

### 5.3. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên CSKH Ban Quản lý, người tiếp nhận và route ticket cư dân. |
| **Workflow** | Nhận ticket, đọc nội dung/ảnh, phân loại, chọn BQL và chuyển tiếp. |
| **Bottleneck** | Đọc văn bản không cấu trúc và đối chiếu danh mục/BQL thủ công. |
| **Impact** | Ước tính 8 phút/ticket, chậm phản hồi và có nguy cơ route sai. |
| **Success Metric** | Giảm xử lý xuống <= 2 phút và route đúng >= 92% trong tập pilot. |
| **Boundary** | Chỉ xử lý triage; không tự trả lời cam kết, không tự quyết định xử lý sự cố, không tự route khi confidence thấp. |

**Cau hoi AI phan bien v0:**
- Field mơ hồ: số liệu 200 ticket/ngày và 8 phút/ticket chưa có log gốc; taxonomy và tiêu chí route đúng chưa chốt.
- Tôi sửa gì: đánh dấu các số liệu là hypothesis, thêm confidence threshold, human review và fallback.

---

## Phase 6 - Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp

- Độ mơ hồ: **[x] Cao** - ticket tiếng Việt có thể có nhiều ý, ảnh đính kèm và thiếu trường.
- Độ phức tạp: **[x] Cao** - nhiều bước, kết hợp extraction, classification, routing và review.

**Bai toan nhom nam o o:**

```text
Cao mơ hồ / Cao phức tạp, nhưng chỉ trong phạm vi triage ticket; không mở rộng thành agent tự xử lý sự cố.
```

### 6.1. So sánh Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| Rule | Keyword, danh mục, danh bạ BQL và required fields | Ticket có mẫu cấu trúc, từ vựng ổn định | Bỏ sót cách diễn đạt tự nhiên, multi-intent | Dùng làm validation và fallback |
| Workflow | Extraction/classification -> confidence -> CSKH review -> route | Đa số ticket có thể triage theo luồng cố định | Sai nhãn hoặc JSON lỗi | **Chọn cho pilot** |
| Agent | Tự lập kế hoạch, gọi nhiều tool, tự xử lý ticket | Quy trình đã có dữ liệu và governance mạnh | Khó audit, route sai, vượt boundary | Không chọn |

**5 cau hoi chot:**
1. Rule xu ly duoc ticket co keyword ro, nhung chua chac dat 70-80% khi van ban tu nhien va multi-intent nhieu.
2. Cac buoc chinh di theo luong thang, co nhanh fallback khi confidence thap.
3. Khong can Agent tu lap ke hoach; workflow co schema va human review la du.
4. CSKH phat hien sai trong buoc review, muc tieu khong qua 20 giay/ticket trong pilot.
5. Co the ha xuong Rule cho danh muc co tu khoa va dung workflow cho phan con lai.

**Muc chon:**

```text
Workflow
```

**Vi sao chon:**

```text
Workflow tach phan AI goi y khoi quyet dinh route cuoi. Schema, confidence threshold va audit log lam cho ket qua co the kiem tra. No phu hop hon Agent vi cac buoc, nguoi review va fallback da biet truoc.
```

**Vi sao khong chon muc don gian hon:**

```text
Rule chi phu hop voi ticket co mau cau truc va tu khoa on dinh, trong khi dau vao la mo ta tu nhien. Tuy nhien nhom van giu Rule cho required fields, keyword va fallback; AI chi xu ly phan Rule khong bao phu.
```

### 6.2. Problem Statement v1

| Field | Noi dung |
|---|---|
| **Actor** | CSKH Ban Quan ly, review goi y truoc khi route ticket cu dan. |
| **Workflow** | CRM nhan ticket; Rule kiem tra input; model trich xuat entity va goi y category/BQL; CSKH review; he thong route. |
| **Bottleneck** | 4-6 phut doc va dien giai noi dung khong cau truc, sau do tra danh muc va BQL. |
| **Impact** | Hypothesis: baseline 8 phut/ticket; muc tieu pilot <= 2 phut, route dung >= 92%. Can log de xac minh. |
| **Success Metric** | Median time/ticket, accuracy route, ty le sua goi y, ty le fallback va ticket bi tra ve. |
| **Boundary** | Lam triage va goi y route. Khong tu tra loi khach, khong tu phan cong ky thuat vien, khong tu dong xu ly ticket confidence thap. |
| **AI intervention point** | Sau Rule kiem tra input va truoc buoc CSKH chon danh muc/BQL. |
| **Muc chon** | Workflow, vi luong co dinh va can ket hop AI voi human review. |
| **Rui ro & nguoi that kiem tra** | Route sai hoac bo sot muc do khan; CSKH review 100% pilot, Ops audit mau hang ngay va co fallback thu cong. |

### 6.3. Final decision

| Cau hoi | Yes / Not Yet / No | Ghi chu |
|---|---|---|
| Actor + workflow ro chua? | Yes | Actor va 5 buoc da duoc gioi han. |
| Baseline + metric do duoc chua? | Not Yet | Co uoc tinh 8 phut va 200 ticket/ngay nhung chua co log goc. |
| Data/input du dung chua? | Not Yet | Can tap ticket an danh, taxonomy va danh ba BQL. |
| AI sai, hau qua chap nhan duoc khong? | Yes, co dieu kien | Chi goi y, CSKH duyet, confidence thap thi fallback. |
| Co nguoi review/owner khong? | Yes | CSKH review; Ops quan ly taxonomy va audit. |
| Co cach non-AI don gian hon khong? | Yes | Rule/required fields la baseline va fallback. |

**Decision:**

```text
Not Yet
```

**Ly do:**

```text
Workflow co actor, bottleneck va metric du kien ro, va co boundary an toan cho human review. Tuy nhien hai so lieu chinh moi la uoc tinh tu bao cao ca nhan, chua co interview, survey hay log ticket de xac minh. Nhom chi nen chuyen sang Go sau khi lay du lieu an danh, chot taxonomy va do baseline tren tap mau.
```

**Neu Go - pilot nho nhat:**

```text
Lay 100-200 ticket da an danh cua mot khu do thi, chi chon 5 danh muc va mot danh ba BQL. Chay song song cach cu va workflow moi, khong tu dong route; do 3 so: median time/ticket, accuracy route va ty le CSKH sua goi y.
```

**Neu Not Yet - can validate gi truoc:**

```text
Phong van 2-3 CSKH/dispatcher do Dương Đức Vương va Nguyễn Ngọc Linh phu trach; thu thap ticket mau da an danh; xac nhan baseline 8 phut, volume va tieu chi route dung; Lê Thị Trâm Anh tong hop ket qua vao bao cao; bo sung cac bao cao ca nhan con thieu.
```

**Neu No-Go - lam gi thay AI:**

```text
Dung form co truong bat buoc, taxonomy nho, keyword rules va danh ba BQL duy nhat; theo doi route sai bang audit hang ngay.
```

**Exit / rollback:**

```text
Tat AI va quay ve Rule + CSKH thu cong neu accuracy route duoi 92% trong hai dot audit lien tiep, ty le sua goi y vuot 20%, co ticket khan bi route sai, schema loi lap lai, hoac AI timeout vuot nguong da dat.
```

---

### Self-check nop phan 02

- [x] Co nhat ky hoi tu tu cac bao cao da nhan, cluster, shortlist va score.
- [ ] Co validation voi quote that; chua co trong input, can bo sung truoc khi Go.
- [x] Co workflow truoc/sau, thoi gian, handoff, bottleneck, boundary va fallback.
- [x] Co PS v0 -> v1, metric truoc/sau va cach do.
- [x] Co so sanh Rule/Workflow/Agent va Decision Not Yet co ly do.
- [ ] Da bo sung candidate ca nhan tu `individual-report3.md`; file hien dang rong.
