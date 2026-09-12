# 02 - Group Problem Statement (Ban nop nhom)

> Ban tong hop tu `individual-report.md` va `indiviual_report2.md`. `individual-report3.md` hien dang rong, vi vay cac candidate ca nhan cua ba thanh vien bo sung chua duoc dien gia.

## Thanh vien nhom

| STT | Ho va ten | Ma hoc vien | Vai tro trong nhom |
|---|---|---|---|
| 1 | Dương Đức Vương | 2A202602944 | Facilitator, validation |
| 2 | Nguyễn Đức Anh Quân | 2A202602405 | Workflow, research |
| 3 | Đỗ Hoàng Quân | 2A202603016 | Domain, AI prototype |
| 4 | Nguyễn Ngọc Linh | 2A202602480 | Research, validation |
| 5 | Lê Thị Trâm Anh | 2A202602846 | Writer, documentation |

**Phan cong bo sung:** Dương Đức Vương phụ trách điều phối và validation; Nguyễn Ngọc Linh phụ trách research và thu thập dữ liệu; Lê Thị Trâm Anh phụ trách viết và chuẩn hóa báo cáo.

**Candidate problem nhom chon (1 cau):**

Nhan vien van hanh phai doc, phan loai va chuyen tiep thong tin khong co cau truc tu nhieu nguon; mot workflow AI co human review co the tao ban tom tat/JSON de giam thoi gian xu ly ma van giu quyen quyet dinh cho nguoi phu trach.

---

## Phase 3 - Group Convergence

### 3.1. Top candidates tu cac bao cao da nhan

| # | Nguoi dua ra | Candidate problem | Nguoi gap van de | Diem nghen | Cam nhan nhanh cua nhom |
|---|---|---|---|---|---|
| 1 | Nguyen Duc Anh Quan | Tong hop task/deadline tu Discord, Zalo, Google Docs | Leader va thanh vien nhom | Doc, doi chieu va gom thong tin tu nhieu kenh | Workflow ro, nhung can gioi han pham vi nguon |
| 2 | Nguyen Duc Anh Quan | Tim lai tai lieu, quyet dinh va file cu truoc deadline | Ca nhom | Search va xac dinh dung phien ban | Pain lap lai, can kho du lieu co quyen truy cap |
| 3 | Nguyen Duc Anh Quan | Viet bao cao/README tu nhieu nguon roi rac | Nguoi viet bao cao | Doc, tom tat, tao draft va sua format | AI phu hop o buoc outline/draft, khong nen tu viet toan bo |
| 4 | Do Hoang Quan | Xu ly su co pin xe Xanh SM va dieu phoi xe sac/cu ho | Dispatcher va tai xe | Doi chieu GPS, tram sac, % pin va soan huong dan | Impact lon, nhung rui ro van hanh va du lieu realtime cao |
| 5 | Do Hoang Quan | Phan loai va dinh tuyen ticket cu dan Vinhomes | CSKH va cu dan | Doc ticket khong cau truc, chon danh muc va BQL | Workflow ro, lap lai cao, do duoc tot |
| 6 | Do Hoang Quan | Chan doan so bo loi xe VinFast tu mo ta tieng Viet | Ky thuat vien va khach hang | Hoi lai trieu chung va tra cuu tai lieu | AI hieu ngon ngu tu nhien, nhung risk sai chan doan cao |
| 7 | Do Hoang Quan | Tong hop ly do khach huy cuoc tu ghi am va ghi chu | BA/Ops | Nghe mau va tim pattern thu cong | Co the mo rong nhung can du lieu ghi am |
| 8 | Do Hoang Quan | Trich xuat release notes tu commit/PR | Ky su, QA va Ops | Hieu commit viet tat va chuyen thanh noi dung de test | Pham vi nho, de lam prototype |
| 9 | Dương Đức Vương, Nguyễn Ngọc Linh, Lê Thị Trâm Anh | Chua co candidate tu bao cao ca nhan | Chua xac dinh | Chua xac dinh | Can bo sung cac bao cao ca nhan |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chu |
|---|---|---|---|
| A - Tong hop tri thuc nhom | 1, 2, 3 | Thong tin roi rac, nguoi dung phai doc va chuyen thanh ban co cau truc | Phu hop workflow AI co review |
| B - Triage va routing van hanh | 4, 5, 6 | Dau vao tu nhien/nhieu he thong, can phan loai va chon hanh dong tiep theo | Can boundary va fallback chat |
| C - Tom tat van hanh | 7, 8 | Chuyen ghi am, commit hoac log thanh summary cho nguoi khac xu ly | De prototype neu co du lieu mau |
| D | 9 | Chua co thong tin | Cho bo sung report 3 |

### 3.3. Shortlist

| Candidate | Vi sao vao shortlist | Rui ro / dieu chua ro |
|---|---|---|
| Phan loai va dinh tuyen ticket cu dan Vinhomes | 200 ticket/ngay theo bao cao; workflow 4 buoc; metric thoi gian va accuracy ro | Chua co tap ticket da an danh; ticket multi-intent chua ro |
| Tong hop task/deadline nhieu kenh | Lap lai 2-3 lan/tuan; pain anh huong ca nhom; co human review tu nhien | Quyen truy cap Discord/Zalo/Docs va nguon su that chua ro |
| Xu ly su co pin nguy cap cho Xanh SM | 80-100 vu/ngay; bottleneck 15 phut; impact doanh thu lon | Ranh gio an toan, API realtime va trach nhiem khi sai cao |

### 3.4. Score de dong thuan

| Candidate | Actor ro | Workflow ro | Pain co evidence | Impact do duoc | Lam trong lab | So sanh R/W/A | Nhom hieu domain | Tong |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Phan loai/routing ticket cu dan | 5 | 5 | 4 | 5 | 4 | 5 | 3 | 31 |
| Tong hop task/deadline nhieu kenh | 5 | 5 | 4 | 4 | 3 | 4 | 4 | 29 |
| Xu ly su co pin nguy cap | 5 | 5 | 4 | 5 | 2 | 3 | 3 | 27 |

**Candidate nhom chon:**

```text
Ho tro phan loai va dinh tuyen ticket phan anh cu dan bang AI, voi CSKH review truoc khi chuyen den BQL phu hop.
```

**Vi sao chon:**

```text
Candidate co actor, dau vao, workflow va dau ra ro rang: CSKH nhan ticket, doc noi dung, phan loai, chon BQL va chuyen tiep. Bao cao ca nhan uoc tinh khoang 200 ticket/ngay/khu do thi va 8 phut/ticket, nen co the do baseline bang thoi gian xu ly, accuracy va ty le route dung. AI phu hop de trich xuat entity va tao JSON, trong khi CSKH van giu quyen review. Pham vi prototype co the gioi han vao mot so danh muc va mot khu do thi.
```

**Vi sao khong chon candidate con lai:**

```text
Tong hop task/deadline tu nhieu kenh co pain ro nhung phu thuoc nhieu nen tang va quyen truy cap, trong khi nhom chua co du lieu lich su de kiem chung. Xu ly su co pin co impact lon nhung sai sot co the gay ton that van hanh va can API realtime, vuot qua pham vi lab hien tai. Cac candidate viet bao cao, tim file va release notes de prototype nhung impact nho hon va chua duoc ca nhom uu tien.
```

**Disagreement:**

```text
Nguyen Duc Anh Quan uu tien bai toan tong hop task vi gan voi workflow hoc tap; Do Hoang Quan uu tien ticket routing vi co volume va metric ro hon. Dương Đức Vương, Nguyễn Ngọc Linh va Lê Thị Trâm Anh tham gia validation, research va chuẩn hóa báo cáo. Nhom tam chot ticket routing theo diem so va kha nang kiem thu, nhung phai xac nhan lai bang validation va bo sung cac bao cao ca nhan con thieu truoc khi Go.
```

---

## Phase 4 - Quick Validation + Research

### 4.1. Quick validation

Chua co interview/survey doc lap trong ba file dau vao. Cac con so duoi day la quan sat/uoc tinh tu ca nhan, khong phai quote da xac minh.

| Nguon | So nguoi/mau | Tin hieu xac nhan | Tin hieu phan bac | Nhom sua problem the nao |
|---|---:|---|---|---|
| Bao cao cua Do Hoang Quan | 1 nguoi quan sat, uoc tinh 200 ticket/ngay | 8 phut/ticket; CSKH doc va chon BQL thu cong | Chua co log/ticket mau | Giu candidate dang hypothesis, gioi han vao ticket mot intent |
| Bao cao cua Nguyen Duc Anh Quan | 1 nhom hoc tap, 4 nguoi | Xac nhan pain chung la thong tin roi rac va can checklist | Khong truc tiep validate ticket cu dan | Dung de so sanh, khong dung lam bang chung domain Vinhomes |
| Interview/survey nguoi dung | Chua thuc hien | Chua co quote nguyen van | Chua co | Can phong van 2-3 CSKH/dispatcher hoac dung tap ticket an danh |

**Insight sau validation:**

```text
Chua du bang chung de ket luan pain 200 ticket/ngay la dai dien cho moi khu do thi. Pain can kiem chung la thoi gian doc va route ticket khong co cau truc; prototype chi nen xu ly mot so danh muc co quy tac ro va luon de CSKH review.
```

### 4.2. Research giai phap da co

| Nguon/tool/case | Link | Ho giai quyet buoc nao? | Diem manh | Khoang trong/rui ro | Bai hoc cho nhom |
|---|---|---|---|---|---|
| Microsoft Power Automate - AI Builder text classification | [Microsoft Learn](https://learn.microsoft.com/en-us/ai-builder/text-classification-overview) | Phan loai text theo nhan | Tich hop workflow va human review | Phu thuoc du lieu huan luyen, multi-intent kho | Bat dau bang classification co nhan |
| Azure AI Language - custom text classification | [Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-services/language-service/custom-text-classification/overview) | Gan nhan danh muc cho van ban | Co custom category va API | Can tap du lieu an danh, theo doi drift | Dinh nghia taxonomy nho va metric F1/accuracy |
| Structured outputs voi Azure OpenAI | [Microsoft Learn](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/structured-outputs) | Trich xuat entity, muc do khan va BQL | JSON de ket noi workflow | JSON hop le khong dong nghia thong tin dung | Validate schema, confidence va buoc review |

**Research takeaway:**

```text
Nen build workflow nho: nhan ticket -> trich xuat truong co cau truc -> goi y danh muc/BQL -> CSKH review -> chuyen tiep. Khong nen build agent tu lap ke hoach, khong nen tu dong chuyen ticket khi confidence thap, va khong nen dua ra cam ket SLA khi chua co du lieu thuc.
```

---

## Phase 5 - Workflow + Problem Statement

### 5.1. Current workflow

```text
[1 Nhan ticket: 1'] -> [2 Doc va hieu noi dung: 4'] -> [3 Chon danh muc/BQL: 2'] -> [4 Gui xac nhan va chuyen ticket: 1']
```

| Buoc | Actor | Input | Output | Thoi gian/tan suat | Ghi chu |
|---|---|---|---|---|---|
| 1 | CSKH | Ticket, anh, thong tin can ho | Ticket duoc mo | 1 phut, hang ngay | Nguon tu App Resident/CRM |
| 2 | CSKH | Mo ta tu nhien, anh dinh kem | Hieu so bo ve van de | 4 phut | Bottleneck; noi dung khong cau truc |
| 3 | CSKH | Noi dung da doc, danh ba BQL | Danh muc va noi nhan | 2 phut | Co the nham voi ticket multi-intent |
| 4 | CSKH/BQL | Ticket da phan loai | Ticket duoc route | 1 phut | Handoff sang BQL |

**Bottleneck chinh:**

```text
CSKH phai doc va dien giai lai van ban tu nhien truoc khi chon danh muc va BQL. Neu thieu thong tin hoac ticket co nhieu y, viec route sai lam tang thoi gian phan hoi; AI chi nen goi y va danh dau do tin cay, khong tu dong quyet dinh moi truong hop.
```

### 5.2. Future workflow

```text
[1 Nhan ticket - he thong] -> [2 Rule kiem tra truong bat buoc] -> [3 AI trich xuat JSON va goi y danh muc/BQL] -> [4 CSKH review, sua neu can - boundary] -> [5 He thong chuyen ticket]

Fallback: confidence < 0.85, schema loi, ticket multi-intent hoac AI timeout thi dua vao hang doi xu ly thu cong; khong tu dong route.
```

**Before/after impact:**

| Metric | Truoc | Sau ky vong | Cach do |
|---|---:|---:|---|
| Thoi gian xu ly ticket | 8 phut | <= 2 phut | Timestamp nhan den route |
| So buoc thu cong | 4 | 1-2 | Dem thao tac cua CSKH |
| Accuracy route | Chua co baseline | >= 92% | So sanh voi nhan dung do reviewer |
| Ticket bi tra ve/sua route | Chua co baseline | Giam 30% | Log route va correction |
| Risk moi | Khong ap dung | AI route sai | Audit mau va fallback |

### 5.3. Problem Statement v0

| Field | Noi dung |
|---|---|
| **Actor** | Nhan vien CSKH Ban Quan ly, nguoi tiep nhan va route ticket cu dan. |
| **Workflow** | Nhan ticket, doc noi dung/anh, phan loai, chon BQL va chuyen tiep. |
| **Bottleneck** | Doc van ban khong cau truc va doi chieu danh muc/BQL thu cong. |
| **Impact** | Uoc tinh 8 phut/ticket, cham phan hoi va co nguy co route sai. |
| **Success Metric** | Giam xu ly xuong <= 2 phut va route dung >= 92% trong tap pilot. |
| **Boundary** | Chi xu ly triage; khong tu tra loi cam ket, khong tu quyet dinh xu ly su co, khong tu route khi confidence thap. |

**Cau hoi AI phan bien v0:**
- Field mo ho: so lieu 200 ticket/ngay va 8 phut/ticket chua co log goc; taxonomy va tieu chi route dung chua chot.
- Toi sua gi: danh dau cac so lieu la hypothesis, them confidence threshold, human review va fallback.

---

## Phase 6 - Rule / Workflow / Agent + Decision

### 6.0. Ma tran do phu hop

- Do mo ho: **[x] Cao** - ticket tieng Viet co the co nhieu y, anh dinh kem va thieu truong.
- Do phuc tap: **[x] Cao** - nhieu buoc, ket hop extraction, classification, routing va review.

**Bai toan nhom nam o o:**

```text
Cao mo ho / Cao phuc tap, nhung chi trong pham vi triage ticket; khong mo rong thanh agent tu xu ly su co.
```

### 6.1. So sanh Rule / Workflow / Agent

| Muc | Phuong an | Khi nao du | Rui ro | Chon? |
|---|---|---|---|---|
| Rule | Keyword, danh muc, danh ba BQL va required fields | Ticket co mau cau truc, tu vung on dinh | Bo sot cach dien dat tu nhien, multi-intent | Dung lam validation va fallback |
| Workflow | Extraction/classification -> confidence -> CSKH review -> route | Da so ticket co the triage theo luong co dinh | Sai nhan hoac JSON loi | **Chon cho pilot** |
| Agent | Tu lap ke hoach, goi nhieu tool, tu xu ly ticket | Quy trinh da co du lieu va governance manh | Kho audit, route sai, vuot boundary | Khong chon |

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
