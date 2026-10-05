# HƯỚNG DẪN THỰC CHIẾN BÀI LAB DAY 18: TỪ PROTOTYPE ĐẾN USER TESTING
*(Dành riêng cho nhóm Tung Tung Tung Sahur: Bá Quân, Việt Anh, Minh Khánh, Quang Huy)*

> **TÌNH TRẠNG HIỆN TẠI**: Nhóm đã phân tích xong 4 Practice Notes và hoàn thành toàn bộ **Chặng 1, 2, 3** (đã được lưu tại [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md) và [README.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/README.md)).  
> Tài liệu này **chỉ tập trung hướng dẫn từng bước làm các phần việc CÒN THIẾU**: từ dựng Prototype, kịch bản test, chạy user testing đến tổng hợp nộp bài.

---

## 🧭 CÁC BƯỚC CẦN THỰC HIỆN TIẾP THEO

```
[ĐÃ XONG]: Chặng 1 (Evidence) ➔ Chặng 2 (3 Options) ➔ Chặng 3 (Human-AI Pass)
                                      ↓
[BƯỚC 1]: Dựng 3 Micro-prototypes trên Figma/Web (Sprint 80 phút)
[BƯỚC 2]: Chốt Kịch bản Outcome Task & Tiêu điểm quan sát (15 phút)
[BƯỚC 3]: 4 Thành viên độc lập Test với 4 Tester ngoài nhóm (20–30 phút)
[BƯỚC 4]: Họp nhóm tổng hợp Ma trận 4 Testers & Chốt Next Change (15 phút)
[BƯỚC 5]: Hoàn thiện 6 files trong Repo cá nhân & Nộp bài (15 phút)
```

---

## 🛠️ BƯỚC 1: DỰNG 3 MICRO-PROTOTYPES (CHẶNG 4 · SPRINT 80 PHÚT)
* **Hình thức**: 👥+👤 Kết hợp (3 bạn dựng 3 Option + 1 bạn dựng Shared Frame)
* **Mục tiêu**: Mỗi option chỉ cần **2–3 màn hình/trạng thái** xoay quanh đúng 1 bài Quiz mẫu.

### 1. Phân công nhiệm vụ cụ thể:
- **Nguyễn Quang Huy (Lead Shared Framework - 15 phút đầu)**:
  - Tạo 1 file Figma chung của nhóm (hoặc Web mockup).
  - Dựng khung **Common Context Screen** (Màn hình câu hỏi Quiz của VLearn) gồm:
    - *Đề bài Quiz chung*: `"Khi cấu hình Virtual Private Cloud (VPC) với dải địa chỉ CIDR 10.0.0.0/16, khẳng định nào sau đây là ĐÚNG về Subnet và số lượng IP khả dụng?"`
    - *4 lựa chọn đáp án A, B, C, D* (có sẵn trạng thái Submit và báo sai màu đỏ).
    - Tạo nút **Reset** ở góc trên để đưa màn hình về trạng thái ban đầu sau mỗi lượt test.
  - Chuẩn bị components chung: Button, Typography, Tag, Toast message.
- **Lại Bá Quân (Lead Option A - In-line Term Inspector)**:
  - Dựng trạng thái: Khi user bôi đen hoặc click vào icon `[?]` cạnh từ khóa `"CIDR 10.0.0.0/16"` hoặc `"VPC"`.
  - Hiển thị popover nổi ngay bên trên từ khóa:  
    *“CIDR /16: Đại diện cho dải mạng lớn có 65,536 IP. Trong bài lab, VPC này đóng vai trò mạng bao quanh toàn bộ hệ thống.”*  
    Kèm icon `[x]` để đóng ngay lập tức (< 5 giây).
- **Nguyễn Thị Minh Khánh (Lead Option B - 30s Diagnostic Micro-Check)**:
  - Dựng trạng thái: Khi user submit đáp án sai, bên cạnh hiện nút `"💡 Chẩn đoán lỗi sai (30s)"`.
  - Khi click vào, hiện modal 2 câu trắc nghiệm 1 chạm:
    - *Câu 1: "Bạn đang phân vân giữa: [A] Số lượng địa chỉ IP hay [B] Quy tắc định tuyến Subnet?"*
    - *Câu 2: "Mục tiêu bài lab bạn muốn: [A] Tạo Subnet công khai hay [B] Tạo Subnet riêng tư?"*
  - Khi user chọn xong, hiện hộp thoại kết luận ngắn gọn:  
    *“Bạn đang nhầm giữa độ dài tiền tố /16 và /24. Số càng nhỏ (/16) thì dải mạng càng lớn. Hãy thử chọn lại đáp án B.”*
  - Luôn có nút `"Bỏ qua chẩn đoán / Đóng"` để thoát.
- **Đỗ Lê Việt Anh (Lead Option C - Proactive Context Action Card)**:
  - Dựng trạng thái: Ngay khi user submit đáp án sai, một thanh trượt / card bên phải **tự động đẩy ra**:
    - *Tiêu đề: "🤖 Gợi ý tự động dựa trên đáp án sai vừa chọn"*
    - *Nội dung: "Có vẻ bạn đang tính nhầm số lượng IP của Subnet /24 thành của cả VPC /16. Trong bài lab này, mỗi Subnet chỉ lấy một phần từ dải /16."*
    - *Nút hành động: `[Xem gợi ý sửa]` và nút `[Bỏ qua / Không cần nhắc lại]`*.

### 2. Kiểm tra chéo nội bộ (15 phút cuối):
- Cả 4 bạn cùng mở file Figma, bấm thử prototype của nhau:
  - Quân bấm thử Option B & C.
  - Khánh bấm thử Option A & C.
  - Anh bấm thử Option A & B.
  - Huy kiểm tra nút **Reset** và lấy link Share (quyền View công khai cho bất kỳ ai có link).
- **Hành động**: Dán đường link Figma/Web vào file [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md).

> 🏁 **CHECKPOINT BƯỚC 1**:
> - [ ] Cả 3 options giải chung 1 câu Quiz về CIDR/VPC do Huy chuẩn bị.
> - [ ] Mỗi option có điểm nhấn Human-AI khác biệt rõ ràng.
> - [ ] Có nút Reset về trạng thái đầu.
> - [ ] Link prototype mở được công khai, không bị chặn quyền.

---

## 📝 BƯỚC 2: CHỐT KỊCH BẢN THỬ NGHIỆM (CHẶNG 5 · 15 PHÚT)
* **Hình thức**: 👥 Cả nhóm dùng chung 1 kịch bản chuẩn
* **Mục tiêu**: Chuẩn bị câu hỏi trung tính, không mớm lời, không bán tính năng.

Nhóm sử dụng kịch bản đã được soạn sẵn sau đây (đã tích hợp vào [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md)):

1. **Câu hỏi Relevant Context (2 phút đầu)**:
   > *"Gần đây khi làm bài tập hoặc lab trên VLearn mà gặp phải một thuật ngữ kỹ thuật khó hiểu hoặc làm sai câu hỏi, việc đầu tiên bạn thường làm là gì?"*

2. **Outcome Task (Giao cho tester khi mở prototype)**:
   > *"Giả sử bạn đang làm bài kiểm tra trên VLearn và vừa chọn sai câu hỏi về VPC/CIDR này. Mục tiêu của bạn là tìm ra lý do mình sai và chọn lại đáp án đúng để hoàn thành bài test. Bạn hãy thao tác thoải mái với giao diện trên màn hình."*  
   *(⚠️ Tuyệt đối không chỉ cho tester bấm vào nút nào! Để họ tự nhìn và bấm).*

3. **5 Tiêu điểm cần quan sát (Observation Focus)**:
   - (1) **First Action**: Mắt họ nhìn vào đâu và tay click vào đâu đầu tiên?
   - (2) **Hesitation / Bối rối**: Chỗ nào họ khựng lại, đọc đi đọc lại hoặc bấm nhầm?
   - (3) **Evidence**: Họ có đọc đoạn giải thích của AI không hay lướt qua luôn?
   - (4) **Control & Recovery**: Họ có tìm thấy và bấm nút đóng/bỏ qua/thử lại không?
   - (5) **Selection & Trade-off**: Sau khi thử cả 3 options, họ chọn A, B hay C và vì sao?

4. **3 Câu Cứu hộ khi Tester bị nghẽn**:
   - *"Bạn cứ nói to những suy nghĩ đang xuất hiện trong đầu nhé."*
   - *"Bây giờ bạn đang muốn làm gì tiếp theo?"*
   - *"Theo suy nghĩ tự nhiên của bạn, chỗ này nó nên phản hồi ra sao?"*

---

## 🧪 BƯỚC 3: TIẾN HÀNH TEST VỚI 4 TESTER ĐỘC LẬP (CHẶNG 6 · 20 PHÚT)
* **Hình thức**: 👤 **CÁ NHÂN ĐỘC LẬP THỰC HIỆN**
* **Mục tiêu**: Mỗi người hẹn 1 bạn ngoài nhóm (ưu tiên học viên khóa 3 hoặc bạn cùng lớp), cho thử **ĐỦ CẢ 3 OPTION A, B, C** và tự ghi chép.

### Phân công 4 phiên test:
- **Lại Bá Quân**: Test với **Tester 1** ➔ Ghi chép vào [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md).
- **Nguyễn Thị Minh Khánh**: Test với **Tester 2** ➔ Ghi chép vào Note cá nhân của Khánh.
- **Đỗ Lê Việt Anh**: Test với **Tester 3** ➔ Ghi chép vào Note cá nhân của Anh.
- **Nguyễn Quang Huy**: Test với **Tester 4** ➔ Ghi chép vào Note cá nhân của Huy.

### Trình tự 20 phút phỏng vấn mỗi tester:
- **Phút 0–2**: Chào hỏi, tạo cảm giác thoải mái (*"Chúng mình đang thử nghiệm vài cách tương tác, test hệ thống chứ không test bạn"*), hỏi câu hỏi Relevant Context.
- **Phút 2–14**: Đưa link prototype, đọc Outcome Task. Cho tester lần lượt trải nghiệm:
  - Cho thử Option A (khoảng 3–4 phút).
  - Bấm Reset, cho thử Option B (khoảng 3–4 phút).
  - Bấm Reset, cho thử Option C (khoảng 3–4 phút).
  *(Quan sát hành vi và ghi chú lại sự ngập ngừng của họ).*
- **Phút 14–18**: Hỏi 3 câu so sánh:
  - *"Trong 3 cách vừa rồi, bạn thấy cách nào giúp bạn hiểu bài và đỡ tốn thời gian nhất? Vì sao?"*
  - *"Bạn thích tự làm phần nào và muốn AI can thiệp vào phần nào?"*
  - *"Điều gì ở phương án bạn chọn khiến bạn vẫn cảm thấy chưa hài lòng?"*
- **Phút 18–20**: Ngồi lại ngay lập tức và điền đầy đủ 4 lớp vào file [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md):
  - **OBSERVED**: Trích dẫn nguyên văn câu tester nói và thao tác họ đã làm.
  - **INTERPRETED**: Bạn giải thích hành vi đó có ý nghĩa gì.
  - **DECIDED**: Đề xuất nhóm nên giữ/bỏ/sửa cái gì ở vòng lặp sau.
  - **STILL UNPROVEN**: Điều gì 1 người này chưa đủ để khẳng định.

> 🏁 **CHECKPOINT BƯỚC 3**:
> - [ ] Cả 4 thành viên hoàn thành 4 phiên với 4 người ngoài nhóm.
> - [ ] Cả 4 tester đều được bấm thử ĐỦ CẢ 3 OPTIONS A, B, C.
> - [ ] Bản ghi chép của bạn [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md) được điền đầy đủ, trung thực.

---

## 🤝 BƯỚC 4: HỌP NHÓM TỔNG HỢP & CHỐT NEXT CHANGE (CHẶNG 7 · 15 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC CẢ NHÓM**
* **Mục tiêu**: Ghép 4 bản ghi chép vào [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md), rút ra bài học chung và chốt 1 quyết định thay đổi tiếp theo.

### Các việc cần làm trong cuộc họp:
1. **Điền ma trận 4 testers**:
   - Từng thành viên đọc tóm tắt: Tester của mình đã bấm gì đầu tiên? Bị nghẽn ở đâu? Chọn option nào và than phiền điều gì?
   - Điền vào bảng so sánh trong [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md).
2. **Tìm Quy luật chung (Pattern) hoặc Khác biệt lớn**:
   - Ví dụ: *"Cả 4 tester đều đánh giá cao tốc độ phản hồi nhưng 3/4 người cảm thấy Option C quá tự tiện nhảy ra gây phiền; đa số nghiêng về Option B vì câu hỏi chẩn đoán giúp họ tự nhận ra lỗi"* hoặc ngược lại.
3. **Chốt 1 Group Next Change duy nhất**:
   - Thống nhất câu trả lời cho: *"Ở phiên bản tiếp theo, nhóm sẽ thay đổi gì?"*
   - *Ví dụ mẫu*: *"Nhóm quyết định chọn Option B làm lõi chính, nhưng sẽ tích hợp tính năng tra cứu từ khóa nhanh của Option A vào các câu hỏi chẩn đoán, đồng thời bổ sung nút 'Bỏ qua xem đáp án ngay' để người dùng không bị ép buộc."*
4. **Ghi rõ Still Unproven**:
   - Thừa nhận thẳng thắn: *"Chưa chứng minh được học viên có tiếp tục dùng công cụ này trong các bài lab dài đòi hỏi gõ lệnh terminal hay không."*

> 🏁 **CHECKPOINT BƯỚC 4**:
> - [ ] Bảng ma trận 4 testers được điền đầy đủ thông tin.
> - [ ] Chốt 1 Next Change dựa trên bằng chứng thực tế, không biểu quyết theo cảm tính.

---

## 📦 BƯỚC 5: HOÀN THIỆN REPO CÁ NHÂN & NỘP BÀI (CHẶNG 8 · 15 PHÚT)
* **Hình thức**: 👤 **CÁ NHÂN TỰ LÀM VÀ NỘP REPO RIÊNG**
* **Tên thư mục / Repo**: `Track1_Day18_02495_LaiBaQuan`

### Checklist 6 files trước khi nộp bài:
- [x] **`README.md`**: Đã điền sẵn thông tin nhóm 4 người, Hypothesis, 3 Options và phần đóng góp của bạn. Bạn chỉ cần cập nhật phần kết quả tổng hợp sau Bước 4.
- [x] **`three-option-design-sheet.md`**: Đã hoàn thành 100% (Chặng 1, 2, 3).
- [ ] **`prototype-link.md`**: Đã dán link Figma/Web công khai từ Bước 1.
- [ ] **`prototype-feedback-note.md`**: Bản ghi chép phiên test với Tester 1 của chính bạn từ Bước 3.
- [ ] **`group-feedback-synthesis.md`**: Bảng tổng hợp 4 testers và Next Change nhóm chốt từ Bước 4.
- [ ] **`ai-support-log.md`**: Tự điền nhật ký dùng AI của bạn (đã có khung mẫu sẵn).

---

## ⚡ HÀNH ĐỘNG NGAY BÂY GIỜ
1. Nhắn cho Huy: *"Huy ơi, mở file Figma chung dựng khung câu hỏi Quiz mẫu VPC/CIDR nhé!"*
2. Bạn (Quân) bắt tay vào vẽ popover giải thích từ khóa cho **Option A**.
3. Nhắn cho Khánh và Anh vào vẽ **Option B** và **Option C**.
4. Hẹn trước 1 người bạn để test lúc kết thúc prototype sprint!
