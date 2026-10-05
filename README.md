# BÁO CÁO LAB DAY 18: TỪ EVIDENCE ĐẾN 3 HUMAN–AI PROTOTYPES

## 1. THÔNG TIN CÁ NHÂN VÀ NHÓM
- **Mã học viên (MHV):** 2A202602495
- **Họ và tên:** Lại Bá Quân
- **Tên nhóm:** Tung Tung Tung Sahur
- **Thành viên trong nhóm & Phân công nhiệm vụ (4 người - mỗi người 1 option):**
  1. **Lại Bá Quân (2A202602495)**: Phụ trách **Option A (Chỉ vào chỗ kẹt - Inline Inspector & Contextual Help)** & Điều phối Tester 1
  2. **Đỗ Lê Việt Anh (2A202602491)**: Phụ trách **Option B (Chẩn đoán 3 câu - 3-Question Diagnostic Micro-Quiz)** & Điều phối Tester 2
  3. **Nguyễn Thị Minh Khánh (2A202602546)**: Phụ trách **Option C (AI gợi ý chủ động - Proactive Nudge Card & Confidence Reasoning)** & Điều phối Tester 3
  4. **Nguyễn Quang Huy (2A202602421)**: Phụ trách **Option D (Hỏi người thật kèm bối cảnh - Human Escalation & Auto Context Docket)** & Điều phối Tester 4
- **Case study được chọn:** AI Tutor: Diagnostic Refresher *(Tiếp tục từ Day 17)*

---

## 2. HYPOTHESIS PROBLEM
- **Vấn đề giả định tiếp tục từ Day 17:**  
  *Học viên trên VLearn gặp bế tắc khi gặp các khái niệm trừu tượng (như Token, Context Window, Tool Calling, Gradient Descent) và lỗi code trong lúc học Slide lý thuyết / làm Lab, dẫn đến việc bị đứt mạch học, mất 30–60 phút phải nhảy ra ngoài ném tài liệu vào ChatGPT (với prompt chưa chuẩn nên nhận về câu trả lời lan man), và thường xuyên không hoàn thành được bài học trong 4 tiếng trên lớp.*
- **Bằng chứng thực tế ban đầu hỗ trợ giả thuyết (từ 4 Practice Notes):**  
  - 100% người học được phỏng vấn (4/4) đều sử dụng ChatGPT bên ngoài như một phương án chữa cháy bắt buộc khi không hiểu bài.
  - Hậu quả thực tế được ghi nhận từ 4 người học: Người học trong phiên của Việt Anh mất 30–60 phút tra cứu ngoài; người học trong phiên của Bá Quân thường xuyên không kịp nộp bài trong ca 4 tiếng; người học trong phiên của Quang Huy chịu áp lực lớn vì prompt chưa chuẩn nên AI trả lời lan man; và người học trong phiên của Minh Khánh khẳng định sẽ bỏ sang ChatGPT nếu công cụ bắt chờ quá 3 phút.
- **Điều quan trọng vẫn chưa được chứng minh:**  
  - Liệu việc đưa sự trợ giúp trực tiếp ngay tại ngữ cảnh bài học (In-context) có thực sự giúp người học hiểu bản chất và làm lab nhanh hơn, hay họ vẫn giữ thói quen copy/paste sang ChatGPT bên ngoài?

---

## 3. FOUR SOLUTION OPTIONS TRONG PROTOTYPE
*(Hiện thực hóa hoàn chỉnh trong mã nguồn [`prototype/index.html`](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype/index.html))*

- **Option A (Chỉ vào chỗ kẹt - Inline Inspector & Contextual Help - Quân lead):**  
  Người học bấm nút *"Tôi vẫn chưa hiểu"* ➔ Màn hình hiện Pickbar ở dưới, các đoạn nội dung/code sáng viền vàng ➔ Chạm chọn đoạn chưa hiểu ➔ Chọn kiểu giúp (*"Giải thích dễ hơn"*, *"Cho ví dụ"*, *"Ôn kiến thức nền"*) hoặc tự gõ câu hỏi ➔ AI hiển thị thẻ `icard` giải thích ngay bên dưới đoạn đó kèm link trích dẫn nguồn bài giảng. *Agency: Don't Act (User-initiated).*
- **Option B (Chẩn đoán 3 câu - 3-Question Diagnostic Micro-Quiz - Việt Anh lead):**  
  Người học bấm nút *"Tôi vẫn chưa hiểu"* ➔ Side panel trượt ra với 3 câu trắc nghiệm 1 chạm (~1 phút) nhằm kiểm tra kiến thức nền ➔ AI đưa ra thẻ chẩn đoán `dcard` phân loại lỗ hổng tri thức, thang đo độ chắc chắn (*Cao / Trung bình / Thấp*), bài ôn có đồ thị SVG minh hoạ trực quan. Cho phép bấm *"Không đúng chỗ"* để tự chọn chủ đề ôn khác. *Agency: Ask (Co-creation).*
- **Option C (AI gợi ý chủ động - Proactive Nudge Card & Confidence Reasoning - Minh Khánh lead):**  
  Hệ thống tự động phát hiện dấu hiệu ngập ngừng (dừng >12 giây trên slide hoặc vừa trả lời sai câu hỏi kiểm tra) ➔ Tự động trượt thẻ `icard nudge` vào đúng khối nghi ngờ kẹt kèm chip tín hiệu hành vi thực tế, mục giải trình minh bạch *"Vì sao AI nghĩ vậy"* và thang đo độ tin cậy. Cho phép bấm *"Đúng chỗ, đã rõ hơn"*, *"Không phải chỗ này"* để chọn lại đoạn bí thật sự, hoặc *"Tắt tự nhắc trong buổi này"*. *Agency: Act (Proactive, User Reviews/Dismisses).*
- **Option D (Hỏi người thật kèm bối cảnh - Human Escalation & Auto Context Docket - Quang Huy lead):**  
  Khi AI chưa thỏa mãn: Người học bấm *"Tôi vẫn chưa hiểu"* ➔ Mở modal tự động thu thập bối cảnh học tập (slide/task đang mở, thời gian kẹt, lịch sử trả lời sai) ➔ Người học tick/untick bảo vệ quyền riêng tư, chọn người gửi (*TA Hà - Mentor lớp* hoặc *Tuấn - Nhóm Lab*) ➔ Gửi yêu cầu và theo dõi tiến trình trong side panel (*Đã gửi ➔ Đã xem ➔ Đang trả lời ➔ Đã trả lời* sau 15 giây mô phỏng). *Agency: Suggest (AI drafts context, User edits & sends).*
- **Link trải nghiệm Prototype:** Xem chi tiết tại [prototype-link.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-link.md). Mở file trực tiếp: [`prototype/index.html`](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype/index.html).
- **Tài liệu phân tích chi tiết của nhóm:** Xem tại [three-option-design-sheet.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/three-option-design-sheet.md).

---

## 4. ĐÓNG GÓP CỦA TÔI TRONG NHÓM (MY CONTRIBUTIONS)
- **Đóng góp Dữ liệu Khảo sát Thực tế (Chặng 1):**
  - Đóng góp Note phỏng vấn cá nhân (Note 3) từ việc phỏng vấn một học viên tự học Cloud/Dev, phát hiện thói quen bỏ video sang làm hands-on lab và nỗi đau không hoàn thành lab trong 4 tiếng trên lớp.
  - Cùng nhóm thảo luận, bóc tách Fact vs. Interpretation và đồng thuận chốt Hypothesis Problem, Comparison Contract cho 4 options.
- **Thiết kế & Triển khai Phương án Phụ trách (Lead Option A - Chặng 2, 3, 4):**
  - **Trực tiếp thiết kế và làm chủ Option A (Chỉ vào chỗ kẹt - Inline Inspector)**: Xác định tương tác chạm khối văn bản/code viền vàng, thanh Pickbar chọn 3 chế độ trợ giúp (*Giải thích dễ hơn, Cho ví dụ, Ôn kiến thức nền*), cơ chế tự soạn câu hỏi và in-line card giải thích ngay tại chỗ với link trích dẫn slide gốc.
  - Phối hợp cùng 3 thành viên (Việt Anh phụ trách Opt B, Minh Khánh phụ trách Opt C, Quang Huy phụ trách Opt D) hiện thực hóa trọn vẹn 4 phương án vào web micro-prototype độc lập tại [`prototype/index.html`](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype/index.html) với 3 chủ đề kiến thức (*Context Window*, *ReAct Agent*, *Gradient Descent*), bộ đo logging tự động và nút Copy CSV.
- **Thử nghiệm & Thu thập dữ liệu Người dùng (Chặng 6):**
  - Trực tiếp điều phối và phỏng vấn độc lập với **Tester 1** (học viên ngoài nhóm) trải nghiệm qua các options; ghi nhận phản ứng với Option A và các phương án so sánh, trích xuất log CSV khách quan vào [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md).
- **Tổng hợp & Phản biện Quyết định Nhóm (Chặng 7):**
  - Cùng nhóm tổng hợp ma trận 4 testers tại [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md) và chốt quyết định *Group Next Change*.

---

## 5. PROTOTYPE FEEDBACK & GROUP SYNTHESIS
- **Ghi chép phiên cá nhân phụ trách (Tester 1):** Xem chi tiết tại [prototype-feedback-note.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype-feedback-note.md).
- **Bảng tổng hợp phản hồi 4 testers của nhóm:** Xem chi tiết tại [group-feedback-synthesis.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/group-feedback-synthesis.md).
- **Quyết định Next Change chung của nhóm:** Lấy tương tác chạm chọn vùng kẹt của **Option A** làm chủ đạo, tích hợp cơ chế kích hoạt thông minh khi làm sai Quiz (rút kinh nghiệm từ Opt C) và micro-diagnostic 1 câu ngắn (~10s) thay vì 3 câu dài (tinh gọn từ Opt B). Tự động đề xuất leo thang sang người thật (**Option D**) khi làm sai quiz quá 2 lần.
- **Những điều Still Unproven (Chưa được chứng minh):** Chưa kiểm chứng được trên các bài lab lập trình code dài/lỗi runtime; chưa đo lường được mức độ ghi nhớ kiến thức dài hạn (Retention); và mẫu thử 4 người còn nhỏ, chưa phản ánh đầy đủ áp lực học sát hạn nộp bài trong thực tế.

---

## 6. AI SUPPORT LOG SUMMARY
- Xem nhật ký khai báo sử dụng AI chi tiết tại [ai-support-log.md](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/ai-support-log.md).
- Tóm tắt: AI hỗ trợ gợi ý cấu trúc phân rã Human-AI, sinh dummy data câu hỏi Quiz và rà soát câu hỏi dẫn dắt trong kịch bản test. 100% dữ liệu phỏng vấn trong 4 Practice Notes và các phiên thử nghiệm đều xuất phát từ học viên thật.
