# HƯỚNG DẪN THỰC HIỆN LAB DAY 18: TỪ EVIDENCE ĐẾN 3 HUMAN–AI PROTOTYPES
*(Phiên bản chuẩn hóa tối ưu dành riêng cho NHÓM 4 THÀNH VIÊN)*

> **Dành cho sinh viên**: Bản hướng dẫn từng bước (Step-by-Step Guide) giúp hoàn thành trọn vẹn bài Lab Day 18 một cách tường minh, đúng chuẩn phương pháp luận Human–AI Design, phân định rõ ràng giữa **Phần việc Cộng tác Nhóm** và **Phần việc Cá nhân**, phân công tối ưu cho **nhóm 4 người**, kèm hệ thống **Checkpoint kiểm tra** và **Tiêu chí đánh giá 5 Gate**.

---

## 📌 BẢN ĐỒ TIẾN TRÌNH & PHÂN ĐỊNH TRÁCH NHIỆM CHO NHÓM 4 NGƯỜI

### 1. Luồng phát triển từ Day 17 sang Day 18 (Quy mô 4 thành viên)
```
[DAY 17: PROBLEM DISCOVERY]
4 Practice Notes + Hypothesis Problem + Solution Parking Lot
                          ↓
[DAY 18: HUMAN–AI PROTOTYPING & USER TESTING]
Chặng 1: Tổng hợp Evidence từ 4 Practice Notes & Chốt Hypothesis Problem
Chặng 2: Chọn 3 Solution Options (A/B/C) + Comparison Contract
Chặng 3: Human–AI Design Pass (Expectation, Agency, Evidence, Recovery)
Chặng 4: Build 3 Micro-prototypes (3 người lead 3 Options + 1 người lead Shared Framework)
Chặng 5: Soạn Kịch bản Outcome Task & 5 Tiêu điểm quan sát
Chặng 6: 4 Thành viên × 4 Tester độc lập ngoài nhóm (mỗi tester trải nghiệm cả A/B/C)
Chặng 7: Group Feedback Synthesis (Tổng hợp 4 bản ghi chú) + Chốt Next Change
Chặng 8: Hoàn thiện 4 Repositories cá nhân & AI Support Log
```

---

### 2. Mô hình phân công vai trò trong Nhóm 4 người

Nhóm vẫn giữ cấu trúc **3 Solution Options (A/B/C)** để bảo đảm đúng chuẩn đề bài và không bị loãng phạm vi. Vai trò của 4 thành viên được phân định mạch lạc như sau:

| Thành viên | Trách nhiệm chính ở Chặng Prototype (Chặng 4) | Trách nhiệm ở Chặng Thử nghiệm (Chặng 6) |
| :--- | :--- | :--- |
| **Thành viên 1** *(Lại Bá Quân)* | **Chủ trì thiết kế Option A** (tập trung cơ chế tương tác A) | Độc lập test Tester 1 (chạy A/B/C) -> Ghi Feedback Note 1 |
| **Thành viên 2** | **Chủ trì thiết kế Option B** (tập trung cơ chế tương tác B) | Độc lập test Tester 2 (chạy A/B/C) -> Ghi Feedback Note 2 |
| **Thành viên 3** | **Chủ trì thiết kế Option C** (tập trung cơ chế tương tác C) | Độc lập test Tester 3 (chạy A/B/C) -> Ghi Feedback Note 3 |
| **Thành viên 4** | **Chủ trì Shared Framework**: Common Context (70%), Data Fixtures, Design Components, cơ chế Reset & kịch bản test | Độc lập test Tester 4 (chạy A/B/C) -> Ghi Feedback Note 4 |

> 💡 **Điểm mạnh của nhóm 4 người**: Có thêm 1 thành viên chuyên trách giữ vững tính đồng nhất (70% Shared Core) giúp 3 Options không bị lệch pha về giao diện/dữ liệu; đồng thời nhóm có tới **4 testers độc lập** ở Chặng 6, giúp dữ liệu phản hồi phong phú và đáng tin cậy hơn rất nhiều!

---

### 3. Bảng phân định công việc: Nhóm (Team) vs. Cá nhân (Individual)

| Chặng | Tên chặng | Thời lượng | Hình thức | Sản phẩm đầu ra |
| :--- | :--- | :--- | :---: | :--- |
| **0** | Chuẩn bị & Thu thập đầu vào Day 17 | 10 phút | 👥+👤 Kết hợp | 4 Practice Notes + Hypothesis sẵn sàng |
| **1** | Tổng hợp Evidence (4 Notes) | 15 phút | 👥 **CỘNG TÁC NHÓM** | Evidence Snapshot + Hypothesis Problem |
| **2** | Chọn 3 Solution Options | 20 phút | 👥 **CỘNG TÁC NHÓM** | Bảng Comparison Contract (A/B/C) |
| **3** | Human–AI Design Pass | 30 phút | 👥 **CỘNG TÁC NHÓM** | Human–AI Decision Table hoàn chỉnh |
| **4** | Build 3 Micro-prototypes | 80 phút | 👥+👤 **KẾT HỢP**<br>*(3 Dev Options + 1 Framework)* | 3 Micro-prototypes hoàn chỉnh, chung 70% |
| **5** | Chuẩn bị Kịch bản Test | 15 phút | 👥 **CỘNG TÁC NHÓM** | Outcome Task + Observation Focus Sheet |
| **6** | Test với 4 Tester độc lập | 20–30 phút | 👤 **CÁ NHÂN ĐỘC LẬP**<br>*(Mỗi người test 1 người)* | 4 Bản Prototype Feedback Note cá nhân |
| **7** | Tổng hợp Group Synthesis | 15 phút | 👥 **CỘNG TÁC NHÓM** | Ma trận 4 testers + 1 Next Change chung |
| **8** | Hoàn thiện Repo & Nộp bài | 20 phút | 👤 **CÁ NHÂN ĐỘC LẬP** | 4 Repositories cá nhân đạt chuẩn |

---

## 🚀 HƯỚNG DẪN CHI TIẾT TỪNG BƯỚC CHO NHÓM 4 NGƯỜI

---

### CHẶNG 0: CHUẨN BỊ ĐẦU VÀO TỪ DAY 17 (10 PHÚT)
* **Hình thức**: 👥+👤 Kết hợp nhóm & cá nhân
* **Mục tiêu**: Tập hợp đủ nguyên liệu từ cả 4 thành viên trước khi bắt tay làm bài.

#### Các bước thực hiện:
1. **Kiểm tra Case study**: Cả 4 thành viên thống nhất tiếp tục giữ nguyên case Day 17 (*AI Tutor*, *AI Notes*, hoặc *AI Support Radar*). **Tuyệt đối không đổi case.**
2. **Đặt 4 nhóm artifacts Day 17 cạnh nhau**:
   - `Hypothesis Problem` của nhóm từ Day 17.
   - **4 Practice Notes** (mỗi thành viên mang đến 1 bản ghi chép phỏng vấn từ Day 17).
   - `Solution Parking Lot` có tối thiểu 5 hướng giải pháp.
   - `Conversation Guide` cuối Day 17 (dùng tra cứu bối cảnh, không phỏng vấn lại).
3. **Mở tài liệu làm việc chung**: Mở file [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md) hoặc board nhóm để cùng điền.

---

### CHẶNG 1: TỔNG HỢP EVIDENCE TỪ 4 PRACTICE NOTES (15 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC NHÓM**
* **Mục tiêu**: Nối giả thuyết vấn đề với bằng chứng thực tế từ 4 cuộc phỏng vấn, phân biệt rạch ròi giữa *Sự thật người dùng nói/làm* và *Diễn giải của nhóm*.

#### Các bước thực hiện:
1. **Họp Evidence Huddle (8 phút)**:
   - Lần lượt **cả 4 thành viên** đọc to 1 chi tiết đắt giá nhất từ Practice Note của mình (nguyên văn câu nói hoặc hành vi thực tế, không suy đoán).
   - Điền vào bảng đối chiếu trong [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md):
     | Practice Note | Người dùng thực sự làm/nói gì? (Raw Fact) | Nhóm đang diễn giải gì? (Interpretation) |
     | :--- | :--- | :--- |
     | **Note 1 (Thành viên 1 - Quân)** | *Ví dụ: "Em thường chụp ảnh bài toán quăng vào chatbot chứ không gõ lại công thức"* | *User ưu tiên tốc độ hơn độ chính xác của đề bài* |
     | **Note 2 (Thành viên 2)** | *...* | *...* |
     | **Note 3 (Thành viên 3)** | *...* | *...* |
     | **Note 4 (Thành viên 4)** | *...* | *...* |

2. **Thảo luận nhanh 4 câu hỏi định hướng (3 phút)**:
   - Trong 4 ghi chú, có thói quen hoặc giải pháp tạm thời (workaround) nào xuất hiện từ 2 lần trở lên?
   - Có chi tiết nào giữa 4 người dùng bị mâu thuẫn hoặc làm nhóm bất ngờ?
   - Điều gì nhóm tin chắc nhưng thực tế chưa có bằng chứng xác thực?

3. **Chốt Hypothesis Problem Statement (4 phút)**:
   - Điền chuẩn form 3 câu:
     - **Hypothesis Problem nhóm tiếp tục**: `[Người dùng X] gặp khó khăn khi [Tình huống Y] dẫn đến [Hậu quả/Nỗi đau Z]`.
     - **Evidence ban đầu hỗ trợ giả thuyết**: `[Trích dẫn 1-2 hành vi thực tế từ 4 ghi chú trên]`.
     - **Điều vẫn chưa được chứng minh**: `[Giả định then chốt cần tiếp tục kiểm chứng hôm nay]`.

> 🏁 **CHECKPOINT 1**:
> - [ ] Đầy đủ bằng chứng từ cả 4 thành viên.
> - [ ] Tách rõ ràng giữa Sự thật (Fact) và Suy diễn (Interpretation).
> - [ ] Hypothesis Problem ngắn gọn, sắc nét, tập trung vào 1 nỗi đau cụ thể.

---

### CHẶNG 2: CHỌN 3 SOLUTION OPTIONS (20 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC NHÓM**
* **Mục tiêu**: Chọn ra đúng 3 phương án (Option A, B, C) cùng giải 1 vấn đề nhưng khác biệt bản chất về cơ chế Human–AI.

#### Các bước thực hiện:
1. **Rà soát Solution Parking Lot (5 phút)**:
   - Mở pool ý tưởng từ Day 17.
   - Nhóm 4 người cùng phản biện: Loại bỏ các ý tưởng chỉ khác nhau về màu sắc, giao diện, hoặc câu từ.
   - Phân bố 3 options đại diện cho các mức độ tự trị khác nhau của AI:
     - **Option A - User Initiates / AI Assists**: Người dùng chủ động bắt đầu, AI hỗ trợ từng phần theo yêu cầu.
     - **Option B - Co-Creation / Collaborative**: Người và AI đối thoại/trao đổi hai chiều qua lại (ví dụ phương pháp Socratic).
     - **Option C - AI Proactive / User Reviews**: AI chủ động phân tích đề xuất trước, Người dùng giữ vai trò thẩm định, duyệt hoặc sửa.

2. **Thiết lập Comparison Contract (10 phút)**:
   - **Những thứ BẮT BUỘC GIỮ NGUYÊN (70% Shared Core)**:
     - *Target User*: Đối tượng mục tiêu cụ thể.
     - *Situation*: Bối cảnh sử dụng.
     - *Task*: Tác vụ cần giải quyết (cùng 1 đề toán, 1 lỗi code, hoặc 1 văn bản).
     - *Desired Outcome*: Kết quả cần đạt được.
     - *Content/Data Fixture*: Dữ liệu mẫu giống hệt nhau ở cả 3 options.
   - **Những thứ ĐƯỢC PHÉP KHÁC NHAU**:
     | Tiêu chí | Option A | Option B | Option C |
     | :--- | :--- | :--- | :--- |
     | **Solution Mechanism** | | | |
     | **User làm gì?** | | | |
     | **AI làm gì?** | | | |
     | **Trigger (Kích hoạt khi nào?)** | | | |
     | **Trade-off chính (Được/Mất gì?)** | | | |

3. **Chạy Distance Check (5 phút)**:
   - Điền 3 câu sau mà **KHÔNG ĐƯỢC nhắc đến màu sắc, layout, hay từ ngữ**:
     - *A khác B vì*: `...`
     - *B khác C vì*: `...`
     - *A khác C vì*: `...`

> 🏁 **CHECKPOINT 2**:
> - [ ] Giữ nguyên 3 options (A/B/C) chuẩn mực, không chia thành 4 options làm loãng bài test.
> - [ ] Cả 3 options giải cùng 1 task trên cùng 1 bộ dữ liệu mẫu.
> - [ ] Vượt qua Distance Check (khác về cơ chế tương tác và quyền kiểm soát).

---

### CHẶNG 3: HUMAN–AI DESIGN PASS (30 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC NHÓM**
* **Mục tiêu**: Định nghĩa rõ 4 trụ cột thiết kế tương tác Human–AI cho khoảnh khắc then chốt (Critical Interaction).

#### Các bước thực hiện:
Nhóm 4 người cùng thảo luận và điền bảng **Human–AI Decision Table** trong [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md):

1. **Expectation**: Trước khi AI xử lý, người dùng có biết trước AI sẽ làm gì không? Giới hạn của AI được thông báo ở đâu?
2. **Role & Agency**: AI sẽ **Act** (Tự làm), **Ask** (Hỏi trước khi làm), hay **Don't Act** (Chờ lệnh)? Nếu AI đoán sai, người dùng bị thiệt hại gì và có dễ nhận ra không?
3. **Evidence & Uncertainty**: AI giải thích căn cứ dựa trên dữ liệu nào? Khi AI không chắc chắn, giao diện thể hiện ra sao?
4. **Control & Recovery**: Nút Edit, Undo, Reject, Stop, Dismiss nằm ở đâu? Nếu gợi ý của AI sai hoàn toàn, người dùng có đường thoát nào để tự làm tiếp không?

> 🏁 **CHECKPOINT 3**:
> - [ ] Đã trả lời trọn vẹn 4 trụ cột cho cả Option A, B và C.
> - [ ] Luôn có lối thoát khẩn cấp (Recovery Path) khi AI sinh kết quả sai/vô nghĩa.

---

### CHẶNG 4: BUILD 3 MICRO-PROTOTYPES (SPRINT 80 PHÚT - PHÂN CÔNG 4 NGƯỜI)
* **Hình thức**: 👥+👤 **KẾT HỢP NHÓM & CÁ NHÂN**
* **Mục tiêu**: Xây dựng 3 micro-prototypes hoàn chỉnh, chia sẻ 70% bối cảnh chung, sẵn sàng đem đi test độc lập.

#### Phân công chuyên trách 4 người trong 80 phút:
* **Phút 0–15 (Khởi động chung & Phân vai)**:
  - **Thành viên 4 (Lead Shared Framework)**: Tạo file Figma chung (hoặc thư mục web mockup), dựng khung **Common Context Screen**, chuẩn bị bộ **Data Fixture** (đề bài mẫu, dữ liệu mẫu) và các nút cơ bản (Header, Back, Reset).
  - **Thành viên 1 (Quân)**: Chuẩn bị luồng màn hình & Canned AI responses cho **Option A**.
  - **Thành viên 2**: Chuẩn bị luồng màn hình & Canned AI responses cho **Option B**.
  - **Thành viên 3**: Chuẩn bị luồng màn hình & Canned AI responses cho **Option C**.

* **Phút 15–55 (Thực hiện song song)**:
  - **Thành viên 1**: Build Option A trên Shared Context của Thành viên 4.
  - **Thành viên 2**: Build Option B trên Shared Context của Thành viên 4.
  - **Thành viên 3**: Build Option C trên Shared Context của Thành viên 4.
  - **Thành viên 4**: Rà soát tính đồng nhất thị giác (typography, button states), chuẩn bị cơ chế **Reset state** cho cả 3 option và soạn sẵn draft kịch bản test (Outcome Task) cho Chặng 5.

* **Phút 55–65 (Hoàn thiện Control & Recovery)**:
  - Thành viên 1, 2, 3 gắn các nút Undo, Edit, Try again, Cancel vào prototype của mình.
  - Thành viên 4 kiểm tra chéo xem các nút Recovery đã hoạt động trơn tru chưa.

* **Phút 65–75 (Kiểm tra chéo nội bộ 4 người)**:
  - Thành viên 1 click thử Option B & C.
  - Thành viên 2 click thử Option A & C.
  - Thành viên 3 click thử Option A & B.
  - Thành viên 4 click test cả A, B, C theo vai trò tester ngây thơ (người chưa biết gì).

* **Phút 75–80 (Chuẩn hóa & Lấy link)**:
  - Cả 4 thành viên kiểm tra link public xem người ngoài có mở được không.
  - Dán link vào file [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md).

> 🏁 **CHECKPOINT 4**:
> - [ ] 3 Options dùng chung 70% bối cảnh và bộ dữ liệu mẫu do Thành viên 4 điều phối.
> - [ ] Mỗi thành viên phụ trách rõ ràng một mảng việc, không dẫm chân lên nhau.
> - [ ] Cả 3 options đều có nút Reset và nút Recovery (sửa/hủy kết quả AI).
> - [ ] Link prototype mở được ẩn danh, sẵn sàng đưa cho người ngoài bấm.

---

### CHẶNG 5: CHUẨN BỊ KỊCH BẢN TEST (15 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC NHÓM**
* **Mục tiêu**: Chuẩn bị bộ câu hỏi và kịch bản test trung tính, không mớm lời, không bán giải pháp.

#### Các bước thực hiện:
1. **Chốt câu hỏi Relevant Context (2 phút đầu phiên test)**:
   - *Ví dụ*: "Khi làm bài tập ở nhà gặp một chỗ vướng mắc không hiểu, bạn thường làm gì đầu tiên?"

2. **Chốt Outcome Task (Dùng chung cho cả 3 Options A, B, C)**:
   - **Nguyên tắc**: Task chỉ mô tả **Mục tiêu cần hoàn thành**, KHÔNG chỉ **Nút nào cần bấm**.
   - ❌ *Sai (Mớm lời)*: "Bạn hãy bấm vào nút bóng đèn màu vàng để AI giải thích nhé."
   - ✅ *Đúng (Outcome task)*: "Giả sử bạn cần tìm ra lỗi sai trong bước giải này để sửa trước khi nộp bài. Hãy dùng công cụ trên màn hình để tìm và sửa lỗi đó."

3. **Thống nhất 5 Tiêu điểm Quan sát (Observation Focus)**:
   - (1) *First Action*: Họ click vào đâu đầu tiên khi màn hình hiện ra?
   - (2) *Hesitation*: Họ khựng lại, do dự hoặc bấm nhầm ở bước nào?
   - (3) *Evidence Read/Ignored*: Họ có đọc phần giải thích của AI không hay lướt qua luôn?
   - (4) *Control & Recovery*: Khi AI làm sai hoặc không đúng ý, họ bấm nút nào để sửa?
   - (5) *Option Selection & Trade-off*: Cuối cùng họ chọn A, B hay C và chấp nhận đánh đổi điều gì?

4. **Nằm lòng 3 Câu Cứu hộ khi Facilitate**:
   - *"Bạn cứ nói to những suy nghĩ đang xuất hiện trong đầu nhé."*
   - *"Tiếp theo bạn dự định sẽ làm gì?"*
   - *"Theo cách nghĩ tự nhiên của bạn, chỗ này nó nên phản hồi như thế nào?"*

> 🏁 **CHECKPOINT 5**:
> - [ ] Outcome Task không lộ tên nút bấm.
> - [ ] Cả 4 thành viên thuộc nằm lòng quy tắc giữ im lặng, không giải thích icon hộ tester.

---

### CHẶNG 6: TEST VỚI 4 TESTER ĐỘC LẬP (20–30 PHÚT HOẶC NGOÀI GIỜ)
* **Hình thức**: 👤 **CÁ NHÂN ĐỘC LẬP THỰC HIỆN**
* **Mục tiêu**: Mỗi thành viên tự tìm 1 người ngoài nhóm, độc lập điều phối và thu thập phản hồi khách quan từ con người thật.

#### Phân công kiểm thử độc lập:
- **Thành viên 1 (Quân)**: Test với **Tester 1** (cho thử đủ A, B, C) -> Viết [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md) của Quân.
- **Thành viên 2**: Test với **Tester 2** (cho thử đủ A, B, C) -> Viết Feedback Note của TV2.
- **Thành viên 3**: Test với **Tester 3** (cho thử đủ A, B, C) -> Viết Feedback Note của TV3.
- **Thành viên 4**: Test với **Tester 4** (cho thử đủ A, B, C) -> Viết Feedback Note của TV4.

> ⚠️ **Quy tắc bất di bất dịch**: Dù bạn chịu trách nhiệm vẽ Option nào, bạn vẫn phải mang **ĐỦ CẢ 3 OPTIONS (A, B, C)** cho tester của bạn trải nghiệm! Không được chỉ mang option mình làm đi test.

#### Timeline 20 phút cho một phiên test cá nhân:
* **0–2 phút**: Tạo không khí thoải mái + hỏi câu hỏi Relevant context.
* **2–14 phút**: Cho tester tự bấm trải nghiệm A, B, C (~4 phút/option), có thể xáo trộn thứ tự để tránh thiên kiến.
* **14–18 phút**: Phỏng vấn so sánh:
  - *"Trong 3 cách vừa thử, bạn thấy cách nào phù hợp nhất với thói quen của bạn? Vì sao?"*
  - *"Bạn muốn tự làm phần việc nào và muốn AI làm phần việc nào?"*
  - *"Điều gì ở phương án bạn chọn khiến bạn chưa thật sự an tâm?"*
* **18–20 phút**: Tự viết ghi chép theo **Mô hình 4 lớp thông tin**:
  - `OBSERVED`: Tester đã bấm gì, nói câu gì nguyên văn?
  - `INTERPRETED`: Bạn nghĩ hành vi đó phản ánh điều gì?
  - `DECIDED`: Đề xuất nhóm nên giữ/sửa/bỏ gì ở vòng lặp tới?
  - `STILL UNPROVEN`: Điều gì 1 tester chưa thể khẳng định chắc chắn?

> 🏁 **CHECKPOINT 6**:
> - [ ] Cả 4 thành viên đã hoàn thành 4 phiên test độc lập với 4 người ngoài nhóm.
> - [ ] Cả 4 tester đều được trải nghiệm đủ 3 Options A, B, C.
> - [ ] Mỗi thành viên có 1 bản Feedback Note riêng của phiên mình phụ trách.

---

### CHẶNG 7: TỔNG HỢP FEEDBACK NHÓM (GROUP SYNTHESIS) (15 PHÚT)
* **Hình thức**: 👥 **CỘNG TÁC NHÓM**
* **Mục tiêu**: Ghép 4 bản ghi chú thành bức tranh tổng thể, tìm quy luật/điểm mâu thuẫn và chốt 1 Group Next Change.

#### Các bước thực hiện:
1. **Lập Bảng Cross-Tester Synthesis (10 phút)**:
   - Mở file [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md) và điền thông tin từ 4 phiên:
     | Tiêu chí | Tester 1 (Quân) | Tester 2 (TV2) | Tester 3 (TV3) | Tester 4 (TV4) | Quy luật chung hoặc Mâu thuẫn |
     | :--- | :--- | :--- | :--- | :--- | :--- |
     | **First Action** | | | | | |
     | **Breakdown chính** | | | | | |
     | **Cách lấy lại control** | | | | | |
     | **Option được chọn** | *[A/B/C]* | *[A/B/C]* | *[A/B/C]* | *[A/B/C]* | *Ví dụ: 3 người chọn B, 1 chọn C* |
     | **Trade-off lớn nhất** | | | | | |

2. **Chốt Group Next Change & Still Unproven (5 phút)**:
   - **Một Next Change nhóm chốt làm tiếp**:  
     `...` *(Ví dụ: Nhóm chọn phát triển sâu Option B, nhưng tích hợp thêm nút xem giải thích chi tiết từ Option A và bổ sung cảnh báo khi AI không chắc chắn).*
   - **Bằng chứng dẫn đến quyết định**: Chỉ rõ hành vi/lời nói nào từ 4 testers khiến nhóm đưa ra quyết định này.
   - **Still Unproven**: Liệt kê những câu hỏi lớn vẫn chưa thể chứng minh (Ví dụ: "Chưa rõ học sinh có duy trì dùng cách này khi đối mặt với bài toán dài hay không").

> 🏁 **CHECKPOINT 7**:
> - [ ] Tổng hợp đủ dữ liệu từ cả 4 testers.
> - [ ] Chốt 1 quyết định Next Change duy nhất dựa trên bằng chứng thực tế, không biểu quyết theo cảm tính.
> - [ ] Thừa nhận trung thực các điểm Still Unproven.

---

### CHẶNG 8: HOÀN THIỆN HỒ SƠ & NỘP BÀI REPO CÁ NHÂN (20 PHÚT)
* **Hình thức**: 👤 **CÁ NHÂN ĐỘC LẬP THỰC HIỆN**
* **Mục tiêu**: Mỗi học viên nộp 1 GitHub repository cá nhân đúng tên, đủ 6 files quy định.

#### Cấu trúc Repository cá nhân của bạn:
Tên repository: `Track1_Day18_02495_LaiBaQuan`
```
Track1_Day18_02495_LaiBaQuan/
├── README.md                      # [CÁ NHÂN] Báo cáo 6 mục (nêu rõ vai trò của bạn trong nhóm 4 người)
├── three-option-design-sheet.md   # [NHÓM DÙNG CHUNG] Chặng 1, 2, 3 (có đủ 4 practice notes)
├── prototype-link.md              # [NHÓM DÙNG CHUNG] Link 3 prototype & kịch bản test
├── prototype-feedback-note.md     # [CÁ NHÂN] Ghi chép phiên test do CHÍNH BẠN chủ trì
├── group-feedback-synthesis.md    # [NHÓM DÙNG CHUNG] Tổng hợp ma trận từ 4 testers & Next Change
└── ai-support-log.md              # [CÁ NHÂN] Nhật ký sử dụng AI trung thực của riêng bạn
```

#### Lưu ý then chốt khi viết `README.md` cá nhân:
- Tại **Mục 1**: Liệt kê đầy đủ danh sách 4 thành viên và vai trò phân công của từng người.
- Tại **Mục 4 (Đóng góp của tôi)**: Nêu cực kỳ chi tiết phần việc bạn đã làm (ví dụ: *chủ trì dựng Option A, chuẩn bị canned responses cho tương tác A, trực tiếp facilitate phiên test với Tester 1, tham gia tổng hợp feedback ma trận 4 testers*).

> 🏁 **CHECKPOINT 8 (HOÀN TẤT TOÀN DIỆN)**:
> - [ ] Đầy đủ 6 files markdown trong repo.
> - [ ] Link prototype mở được công khai với giảng viên/mentor.
> - [ ] Báo cáo cá nhân phản ánh đúng vai trò trong nhóm 4 người, tuyệt đối không sao chép nguyên văn phần đóng góp của bạn cùng nhóm.
> - [ ] 100% dữ liệu phỏng vấn đến từ con người thật, không dùng AI bịa đặt.

---

## ⚖️ HỆ THỐNG 5 GATE ĐÁNH GIÁ (RUBRIC CHẤM ĐIỂM)

| Gate đánh giá | Tiêu chuẩn ĐẠT (Pass) | Dấu hiệu KHÔNG ĐẠT (Fail) |
| :--- | :--- | :--- |
| **Gate 1: Evidence Continuity** | Hypothesis Problem xuất phát từ ít nhất 1 observation trong 4 Practice Notes Day 17; ghi rõ điều chưa chứng minh. | Kể lại ý tưởng viển vông; ngộ nhận Practice Notes Day 17 là bài toán đã được validate hoàn toàn. |
| **Gate 2: Meaningful Options** | 3 Options cùng giải 1 vấn đề/tác vụ nhưng khác biệt bản chất về cơ chế và quyền kiểm soát Human–AI. | 3 Options chỉ khác nhau màu nút, đổi layout, hoặc thay đổi vài câu từ. |
| **Gate 3: Human Control** | Mỗi option thể hiện rõ kỳ vọng, mức độ tự trị (Act/Ask/Don't Act), bằng chứng giải thích và có đường phục hồi (recovery). | AI tự ý làm thay người dùng mà không có cách nào ngăn chặn, hoàn tác hoặc sửa đổi khi AI làm sai. |
| **Gate 4: Test-Ready** | Người ngoài nhóm tự mở và bấm trải nghiệm cả 3 options độc lập mà không cần tác giả "thuyết minh hộ". | Người kiểm thử bị tắc đường, prototype không bấm được, hoặc Option do mình làm được chăm chút xịn hơn hẳn 2 option còn lại. |
| **Gate 5: Learning & Synthesis** | Có đủ 4 Feedback Notes, chỉ ra quy luật/mâu thuẫn, chốt 1 Next Change và thừa nhận các điểm Still Unproven. | Chỉ đếm phiếu bầu "3/4 người thích B"; vội vã tuyên bố giải pháp đã hoàn toàn thành công ngoài thị trường. |
