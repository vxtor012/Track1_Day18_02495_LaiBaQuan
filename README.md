# BÁO CÁO LAB DAY 18: TỪ EVIDENCE ĐẾN 3 HUMAN–AI PROTOTYPES

## 1. THÔNG TIN CÁ NHÂN VÀ NHÓM
- **Mã học viên (MHV):** 2A202602495
- **Họ và tên:** Lại Bá Quân
- **Tên nhóm:** Tung Tung Tung Sahur
- **Thành viên trong nhóm (4 người):**
  1. Lại Bá Quân (2A202602495) - Phụ trách Shared Framework (Common Context 70%, Data Fixture, Shared UI Components, Reset Path & Test Script) & Facilitator Tester 1
  2. Nguyễn Thị Minh Khánh (2A202602546) - Phụ trách chính Option A: In-line Term Inspector & Facilitator Tester 2
  3. Đỗ Lê Việt Anh (2A202602491) - Phụ trách chính Option B: 30s Diagnostic Micro-Check & Facilitator Tester 3
  4. Nguyễn Quang Huy (2A202602421) - Phụ trách chính Option C: Proactive Context Action Card & Facilitator Tester 4
- **Case study được chọn:** AI Tutor: Diagnostic Refresher *(Tiếp tục từ Day 17)*

---

## 2. HYPOTHESIS PROBLEM
- **Vấn đề giả định tiếp tục từ Day 17:**  
  *Học viên trên VLearn gặp bế tắc khi gặp các thuật ngữ viết tắt và khái niệm kỹ thuật trừu tượng trong lúc làm Quiz / thực hành Lab, dẫn đến việc bị đứt mạch học, mất 30–60 phút phải nhảy ra ngoài ném tài liệu vào ChatGPT (với prompt chưa chuẩn nên nhận về câu trả lời lan man), và thường xuyên không hoàn thành được bài học trong 4 tiếng trên lớp.*
- **Bằng chứng thực tế ban đầu hỗ trợ giả thuyết (từ 4 Practice Notes):**  
  - 100% người học được phỏng vấn (4/4) đều sử dụng ChatGPT bên ngoài như một phương án chữa cháy bắt buộc khi không hiểu bài.
  - Hậu quả thực tế được ghi nhận từ 4 người học: Người học trong phiên của Việt Anh mất 30–60 phút tra cứu ngoài; người học trong phiên của Bá Quân thường xuyên không kịp nộp bài trong ca 4 tiếng; người học trong phiên của Quang Huy chịu áp lực lớn vì prompt chưa chuẩn nên AI trả lời lan man; và người học trong phiên của Minh Khánh khẳng định sẽ bỏ sang ChatGPT nếu công cụ bắt chờ quá 3 phút.
- **Điều quan trọng vẫn chưa được chứng minh:**  
  - Liệu việc giải thích khái niệm trực tiếp ngay tại bài học (In-context) có thực sự giúp người học hoàn thành bài lab nhanh hơn, hay họ vẫn giữ thói quen copy/paste sang ChatGPT bên ngoài?

---

## 3. THREE SOLUTION OPTIONS (TÓM TẮT 3 PHƯƠNG ÁN)
- **Option A (In-line Term Inspector):** Người dùng bôi đen hoặc click vào từ khóa viết tắt "CIDR / VPC" ➔ Popover mở tức thì giải thích ý nghĩa + 1 ví dụ thực tế trong 1 dòng (< 5 giây). *Agency: Don't Act (User-initiated).*
- **Option B (30s Diagnostic Micro-Check):** Khi làm sai Quiz, AI đưa ra 2 câu trắc nghiệm 1-chạm chẩn đoán điểm hiểu sai ➔ Người dùng bấm chọn nhanh ➔ Nhận tóm tắt đánh trúng điểm nghẽn (< 45 giây). *Agency: Ask (Co-creation).*
- **Option C (Proactive Context Action Card):** Khi làm sai Quiz hoặc dừng quá lâu, AI tự động đẩy thẻ phân tích lỗi và đề xuất cách sửa code/chọn lại bài. *Agency: Act (Proactive, User Reviews/Dismisses).*
- **Link trải nghiệm Prototype (A/B/C):** Xem chi tiết tại [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md).
- **Tài liệu phân tích chi tiết của nhóm:** Xem tại [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md).

---

## 4. ĐÓNG GÓP CỦA TÔI TRONG NHÓM (MY CONTRIBUTIONS)
- **Thiết kế & Prototype:**
  - Đóng góp Note phỏng vấn cá nhân (Note 3) phát hiện thói quen bỏ video sang làm hands-on lab và nỗi đau không hoàn thành lab trong 4 tiếng.
  - Cùng nhóm thảo luận, bóc tách Fact vs. Diễn giải và chốt Hypothesis Problem, Comparison Contract cho 3 Options.
  - **Trực tiếp phụ trách xây dựng Shared Framework & Common Context (70% shared core)**:
    - Thiết lập khung màn hình VLearn với bài toán Quiz mẫu (VPC & CIDR Block) dùng chung cho cả 3 options.
    - Chuẩn hóa bộ Design Tokens, UI components (Buttons, Typography, State tags, Popovers).
    - Thiết kế cơ chế Reset trạng thái và tích hợp liên kết điều hướng mượt mà cho 3 Option A, B, C.
    - Soạn thảo và chuẩn hóa kịch bản Outcome Task & 5 Tiêu điểm quan sát.
- **Thử nghiệm & Thu thập dữ liệu:**
  - Trực tiếp điều phối và phỏng vấn độc lập với **Tester 1** (học viên ngoài nhóm) trải nghiệm đủ cả 3 Option A, B, C; hoàn thành bản ghi chép chi tiết [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md).
- **Tổng hợp & Phản biện:**
  - Cùng nhóm phân tích ma trận 4 testers tại [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md) và chốt quyết định *Group Next Change*.

---

## 5. PROTOTYPE FEEDBACK & GROUP SYNTHESIS
- **Ghi chép phiên cá nhân phụ trách (Tester 1):** Xem chi tiết tại [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md).
- **Bảng tổng hợp phản hồi 4 testers của nhóm:** Xem chi tiết tại [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md).
- **Quyết định Next Change chung của nhóm:** *(Sẽ được nhóm chốt sau khi hoàn thành Chặng 6 & 7)*.
- **Những điều Still Unproven (Chưa được chứng minh):** *(Sẽ được nhóm chốt sau khi hoàn thành Chặng 6 & 7)*.

---

## 6. AI SUPPORT LOG SUMMARY
- Xem nhật ký khai báo sử dụng AI chi tiết tại [ai-support-log.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/ai-support-log.md).
- Tóm tắt: AI hỗ trợ gợi ý cấu trúc phân rã Human-AI, sinh dummy data câu hỏi Quiz và rà soát câu hỏi dẫn dắt trong kịch bản test. 100% dữ liệu phỏng vấn trong 4 Practice Notes và các phiên thử nghiệm đều xuất phát từ học viên thật.
