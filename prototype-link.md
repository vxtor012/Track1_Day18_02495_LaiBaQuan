# PROTOTYPE LINKS & TEST CONTEXT (NHÓM TUNG TUNG TUNG SAHUR)

> **Tài liệu truy cập Prototype chung của nhóm**: Chứa đường link nguyên mẫu của cả 3 Option và kịch bản kiểm thử đã được chuẩn hóa cho bài toán Quiz VLearn.

---

## 1. ĐƯỜNG LINK TRẢI NGHIỆM PROTOTYPE (A / B / C)

- **Công cụ xây dựng:** Figma / Web Mockup
- **Đường link chung (hoặc link từng Option):**
  - **Link Figma Prototype chung của nhóm:** `[Dán link Figma của nhóm tại đây - Nhớ bật quyền Anyone with the link can VIEW]`
  - **Option A (In-line Term Inspector):** `[Dán link frame Option A]`
  - **Option B (30s Diagnostic Micro-Check):** `[Dán link frame Option B]`
  - **Option C (Proactive Context Action Card):** `[Dán link frame Option C]`

---

## 2. KỊCH BẢN THỬ NGHIỆM ĐÃ CHUẨN HÓA (CHẶNG 5)

### Bối cảnh bài kiểm tra mẫu (Common Context & Data Fixture)
- **Câu hỏi Quiz mẫu trên VLearn:**  
  *"Khi khởi tạo một Virtual Private Cloud (VPC) với dải địa chỉ CIDR `10.0.0.0/16`, phát biểu nào sau đây là ĐÚNG về Subnet và số lượng IP khả dụng?"*
- **4 Lựa chọn:**
  - A. Dải mạng này chỉ cấp phát được tối đa 256 địa chỉ IP cho toàn bộ VPC.
  - B. Dải mạng cung cấp 65,536 địa chỉ IP, và các Subnet con có thể chia theo tiền tố `/24` để phân chia mạng. *(Đáp án đúng)*
  - C. Subnet bắt buộc phải có cùng kích thước tiền tố `/16` với VPC cha. *(Học viên chọn nhầm câu này và bị báo sai)*
  - D. Không thể gán Subnet cho VPC khi đã chỉ định CIDR.

---

### Câu hỏi Relevant Context (2 phút đầu phiên test):
> *"Gần đây khi làm bài tập hoặc Quiz trên VLearn mà gặp phải một thuật ngữ kỹ thuật khó hiểu hoặc làm sai câu hỏi, việc đầu tiên bạn thường làm là gì?"*

### Outcome Task (Giao cho tester khi mở prototype):
> *"Giả sử bạn đang làm bài kiểm tra trên VLearn và vừa chọn sai câu hỏi về VPC/CIDR này. Mục tiêu của bạn là tìm ra lý do mình sai và chọn lại đáp án đúng để hoàn thành bài test. Bạn hãy thao tác tự nhiên với giao diện trên màn hình."*  
*(⚠️ Lưu ý người facilitate: Tuyệt đối không chỉ cho tester bấm vào nút nào! Để họ tự nhìn và bấm).*

### 5 Tiêu điểm quan sát (Observation Focus):
1. **First action:** Mắt và tay họ click vào đâu đầu tiên khi thấy màn hình kết quả sai?
2. **Hesitation / Bối rối:** Chỗ nào họ khựng lại, đọc đi đọc lại hoặc bấm nhầm?
3. **Evidence:** Họ có đọc phần giải thích của AI không hay lướt qua luôn?
4. **Control & Recovery:** Họ có tìm thấy và bấm nút đóng/bỏ qua/thử lại không?
5. **Trade-off:** Sau khi thử cả 3 options, họ chọn A, B hay C và vì sao?

### 3 Câu Cứu hộ khi Tester bị nghẽn:
- *"Bạn cứ nói to những suy nghĩ đang xuất hiện trong đầu nhé."*
- *"Bây giờ bạn đang muốn làm gì tiếp theo?"*
- *"Theo suy nghĩ tự nhiên của bạn, chỗ này nó nên phản hồi ra sao?"*
