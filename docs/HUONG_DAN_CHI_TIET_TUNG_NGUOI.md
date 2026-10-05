# HƯỚNG DẪN CHI TIẾT TỪNG NGƯỜI (NHÓM TUNG TUNG TUNG SAHUR)

> **Phân công nhiệm vụ chính thức**:  
> - 👑 **Lại Bá Quân (2A202602495)**: Lead Shared Framework, Common Context, UI Components, Reset Path & Điều phối kịch bản  
> - 🎨 **Nguyễn Thị Minh Khánh (2A202602546)**: Triển khai Option A (In-line Term Inspector)  
> - 🧩 **Đỗ Lê Việt Anh (2A202602491)**: Triển khai Option B (30s Diagnostic Micro-Check)  
> - 🤖 **Nguyễn Quang Huy (2A202602421)**: Triển khai Option C (Proactive Context Action Card)  

---

## 📌 BẢNG TỔNG HỢP VAI TRÒ & DEADLINE

| Thành viên | Trách nhiệm Prototype (Chặng 4 · 80p) | Trách nhiệm Thử nghiệm (Chặng 6 · 20p) | Sản phẩm cá nhân phải nộp |
| :--- | :--- | :--- | :--- |
| **1. Lại Bá Quân** | Dựng khung Common Context (Figma), Data Fixture Quiz mẫu, components, nút Reset & ghép luồng chung | Facilitate **Tester 1** (cho thử A/B/C) ➔ Ghi chép cá nhân | Repo cá nhân đầy đủ 6 files chuẩn |
| **2. Minh Khánh** | Dựng tương tác **Option A**: Popover tra cứu từ khóa tức thì khi click vào text (<5s) | Facilitate **Tester 2** (cho thử A/B/C) ➔ Ghi chép cá nhân | Repo cá nhân đầy đủ 6 files chuẩn |
| **3. Việt Anh** | Dựng tương tác **Option B**: Modal 2 câu trắc nghiệm 1 chạm chẩn đoán lỗi sai (<45s) | Facilitate **Tester 3** (cho thử A/B/C) ➔ Ghi chép cá nhân | Repo cá nhân đầy đủ 6 files chuẩn |
| **4. Quang Huy** | Dựng tương tác **Option C**: Thẻ Action Card tự động trượt ra phân tích lỗi khi submit sai | Facilitate **Tester 4** (cho thử A/B/C) ➔ Ghi chép cá nhân | Repo cá nhân đầy đủ 6 files chuẩn |

---

## 👤 1. HƯỚNG DẪN DÀNH CHO LẠI BÁ QUÂN (LEAD SHARED FRAMEWORK)

### Nhiệm vụ 1: Dựng nền tảng dùng chung trên Figma (15 phút đầu Chặng 4)
1. **Tạo Figma chung**: Tạo 1 project Figma, đặt tên: `Track1_Day18_TungTungTungSahur_Prototypes`, mời Khánh, Anh, Huy vào với quyền **Editor**.
2. **Dựng màn hình Common Context (70% shared core)**:
   - Dựng giao diện bài học VLearn (chủ đề Cloud / VPC).
   - Đặt câu hỏi Quiz mẫu chuẩn của nhóm:  
     *“Khi khởi tạo một Virtual Private Cloud (VPC) với dải địa chỉ CIDR `10.0.0.0/16`, phát biểu nào sau đây là ĐÚNG về Subnet và số lượng IP khả dụng?”*
   - Dựng 4 đáp án (A, B, C, D) như đã chuẩn hóa trong `prototype-link.md`.
   - Tạo trạng thái người học chọn đáp án sai (Đáp án C) và bấm nút **"Nộp bài"** ➔ Hệ thống báo viền đỏ "Chưa chính xác!".
3. **Dựng các Components chung**:
   - Nút `[Bỏ qua / Đóng / Thử lại]` đồng bộ kích thước và màu sắc.
   - Nút **`[🔄 Reset Prototype]`** đặt cố định ở góc trên bên phải màn hình để đưa về trạng thái đầu.

### Nhiệm vụ 2: Tích hợp và Rà soát Prototype (15 phút cuối Chặng 4)
- Ghép 3 màn hình tương tác do Khánh (Option A), Anh (Option B) và Huy (Option C) vừa vẽ xong vào luồng chung.
- Kiểm tra tính năng nút **Reset** trên cả 3 option.
- Bật quyền Share: **"Anyone with the link can view"** và dán link vào file [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md).

### Nhiệm vụ 3: Độc lập Test với Tester 1 (Chặng 6)
- Tìm 1 bạn học viên ngoài nhóm.
- Đưa link prototype, đọc kịch bản Outcome Task (chỉ nói mục tiêu sửa lỗi, không chỉ nút bấm).
- Cho Tester 1 trải nghiệm lần lượt: **Option A ➔ Reset ➔ Option B ➔ Reset ➔ Option C**.
- Ghi chép ngay lập tức vào file [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md) theo 4 lớp: *Observed / Interpreted / Decided / Still Unproven*.

### Nhiệm vụ 4: Chủ trì họp nhóm tổng hợp & Nộp bài (Chặng 7 & 8)
- Mở cuộc họp ngắn 15 phút, yêu cầu Khánh, Anh, Huy báo cáo tóm tắt phiên test của họ.
- Điền đầy đủ vào bảng [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md) và chốt **1 Group Next Change**.
- Đẩy commit repo cá nhân lên GitHub.

---

## 👤 2. HƯỚNG DẪN DÀNH CHO NGUYỄN THỊ MINH KHÁNH (LEAD OPTION A)

### Nhiệm vụ 1: Xây dựng Option A (In-line Term Inspector) (Chặng 4)
- **Cơ chế**: Tra cứu tức thì từ khóa viết tắt tại chỗ theo yêu cầu của người dùng (User-initiated, không tự ý nhảy ra).
- **Thực hiện trên Figma (sử dụng khung của Quân)**:
  1. Nhân bản (Duplicate) khung màn hình Quiz từ Quân.
  2. Thêm chỉ báo thị giác (Visual affordance): Gạch chân đứt nét màu xanh nhạt hoặc icon `[?]` nhỏ ngay cạnh các từ khóa: `"CIDR 10.0.0.0/16"` và `"VPC"`.
  3. Dựng trạng thái Popover (Tooltip nổi) khi người dùng click vào từ khóa:
     - **Tiêu đề**: *CIDR Block /16*
     - **Giải thích nhanh**: *“Đại diện cho dải mạng lớn gồm 65,536 địa chỉ IP. Trong bài lab này, VPC đóng vai trò là mạng bao quanh toàn bộ hệ thống.”*
     - **Ví dụ thực tế**: *“Một Subnet con thường chia theo /24 (256 IP) để cấp cho các máy ảo con.”*
     - **Nút điều khiển**: Nút icon `[x]` ở góc popover hoặc bấm ra ngoài để đóng ngay lập tức.
- **Thời gian hoàn thành**: 40 phút. Sau khi xong, click thử nghiệm chéo Option B của Anh và Option C của Huy.

### Nhiệm vụ 2: Độc lập Test với Tester 2 (Chặng 6)
- Hẹn trước 1 bạn ngoài nhóm (Tester 2).
- Mở link prototype chung, cho Tester 2 trải nghiệm **cả 3 Option A, B, C** (mỗi option 3-4 phút).
- Quan sát xem họ có nhìn thấy từ gạch chân để click không, có đọc popover không.
- Tự hoàn thành file `prototype-feedback-note.md` trong repo cá nhân của Khánh.

### Nhiệm vụ 3: Tham gia họp nhóm & Nộp bài (Chặng 7 & 8)
- Cung cấp kết quả của Tester 2 cho Quân điền vào ma trận nhóm.
- Đẩy repo cá nhân `Track1_Day18_2A202602546_NguyenThiMinhKhanh`.

---

## 👤 3. HƯỚNG DẪN DÀNH CHO ĐỖ LÊ VIỆT ANH (LEAD OPTION B)

### Nhiệm vụ 1: Xây dựng Option B (30s Diagnostic Micro-Check) (Chặng 4)
- **Cơ chế**: AI chẩn đoán 2 câu trắc nghiệm 1 chạm để bóc tách chỗ hiểu sai trước khi giải thích (Human–AI Co-Creation).
- **Thực hiện trên Figma (sử dụng khung của Quân)**:
  1. Nhân bản khung màn hình Quiz từ Quân.
  2. Tại trạng thái Quiz báo sai, thiết kế 1 nút bấm nổi bật: **`[💡 Chẩn đoán lỗi sai trong 30s]`** đặt cạnh kết quả sai.
  3. Khi click nút này, hiện Modal popup / Bottom sheet:
     - **Bước 1 (Câu hỏi 1)**: *"Bạn đang phân vân nhất ở điểm nào?"*
       - [Nút chọn A]: *Số lượng IP của dải mạng /16*
       - [Nút chọn B]: *Quan hệ giữa Subnet con và VPC cha*
     - **Bước 2 (Câu hỏi 2)**: *"Trong bài lab, bạn dự định tạo Subnet kiểu gì?"*
       - [Nút chọn A]: *Chia nhỏ dải mạng thành nhiều lớp mạng /24*
       - [Nút chọn B]: *Để nguyên cả dải /16 cho 1 máy ảo duy nhất*
  4. Trạng thái kết luận chẩn đoán:
     - Hiển thị thông điệp trúng đích: *“Chẩn đoán: Bạn đang nhầm lẫn giữa quy mô của VPC (/16) và Subnet (/24). Một VPC lớn chứa được nhiều Subnet nhỏ. Hãy thử chọn lại đáp án B nhé!”*
  5. **Nút thoát (Recovery)**: Luôn có nút `[Bỏ qua chẩn đoán / Đóng]` ở mọi bước để người học không bị kẹt.
- **Thời gian hoàn thành**: 40 phút. Sau khi xong, click thử nghiệm chéo Option A của Khánh và Option C của Huy.

### Nhiệm vụ 2: Độc lập Test với Tester 3 (Chặng 6)
- Hẹn 1 bạn ngoài nhóm (Tester 3).
- Cho Tester 3 trải nghiệm đủ cả A, B, C.
- Quan sát: Họ có ngại bấm 2 câu trắc nghiệm không? Họ có thấy câu hỏi chẩn đoán giúp họ ngộ ra lỗi sai không?
- Tự hoàn thành file `prototype-feedback-note.md` trong repo cá nhân của Anh.

### Nhiệm vụ 3: Tham gia họp nhóm & Nộp bài (Chặng 7 & 8)
- Đóng góp insight của Tester 3 vào cuộc họp tổng hợp.
- Đẩy repo cá nhân `Track1_Day18_2A202602491_DoLeVietAnh`.

---

## 👤 4. HƯỚNG DẪN DÀNH CHO NGUYỄN QUANG HUY (LEAD OPTION C)

### Nhiệm vụ 1: Xây dựng Option C (Proactive Context Action Card) (Chặng 4)
- **Cơ chế**: AI chủ động phân tích lỗi sai và đẩy thẻ gợi ý ra màn hình ngay khi submit bài sai (AI Proactive, User Reviews/Dismisses).
- **Thực hiện trên Figma (sử dụng khung của Quân)**:
  1. Nhân bản khung màn hình Quiz từ Quân.
  2. Dựng trạng thái: Ngay khi user bấm nút "Nộp bài" và bị báo sai, ở thanh sidebar bên phải **tự động trượt ra (slide-in) một Thẻ gợi ý (Action Card)**:
     - **Header**: `[🤖 AI Tutor Assistance - Tự động phát hiện điểm nghẽn]`
     - **Phân tích lỗi**: *“Dựa vào việc bạn chọn đáp án C, hệ thống nhận thấy bạn đang nghĩ Subnet phải có cùng dải /16 với VPC.”*
     - **Gợi ý hành động**: *“Trong thực tế Cloud, VPC /16 là mạng cha bao quanh, còn Subnet là các mạng con được chia nhỏ theo tiền tố /24.”*
     - **Hai nút bấm quyết định (Control)**:
       - Nút chính: `[Áp dụng gợi ý & Chọn lại đáp án]`
       - Nút phụ: `[Bỏ qua / Không hiển thị lại]` (để đóng thẻ nếu người học cảm thấy bị làm phiền).
- **Thời gian hoàn thành**: 40 phút. Sau khi xong, click thử nghiệm chéo Option A của Khánh và Option B của Anh.

### Nhiệm vụ 2: Độc lập Test với Tester 4 (Chặng 6)
- Hẹn 1 bạn ngoài nhóm (Tester 4).
- Cho Tester 4 trải nghiệm đủ cả A, B, C.
- Quan sát: Họ có thấy thẻ gợi ý tự động nhảy ra là hữu ích hay là phiền toái? Họ bấm nút áp dụng hay bấm nút tắt đi?
- Tự hoàn thành file `prototype-feedback-note.md` trong repo cá nhân của Huy.

### Nhiệm vụ 3: Tham gia họp nhóm & Nộp bài (Chặng 7 & 8)
- Đóng góp insight của Tester 4 vào ma trận tổng hợp của nhóm.
- Đẩy repo cá nhân `Track1_Day18_2A202602421_NguyenQuangHuy`.

---

## ⚡ TỔNG KẾT: CÁCH PHỐI HỢP NHỊP NHÀNG
1. **Quân** tạo Figma file ngay bây giờ và gửi link cho **Khánh, Anh, Huy**.
2. **Khánh, Anh, Huy** nhân bản frame và bắt tay vào vẽ **Option A, B, C** theo đúng mô tả ở trên.
3. Trong lúc chờ vẽ xong, **cả 4 bạn nhắn tin hẹn ngay 4 người bạn ngoài nhóm** để test cho Chặng 6!
