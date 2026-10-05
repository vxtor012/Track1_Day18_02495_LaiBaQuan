# AI SUPPORT LOG (NHẬT KÝ SỬ DỤNG AI CÁ NHÂN)

> **Học viên:** Lại Bá Quân (2A202602495)
> **Cam kết liêm chính học thuật**: Tôi cam đoan không dùng AI để tạo giả bất kỳ trích dẫn (quote), quan sát (observation) hay phản hồi (feedback) nào của người dùng. Mọi tương tác thử nghiệm đều được tiến hành với con người thật. Phần dưới đây khai báo trung thực các khía cạnh tôi đã sử dụng AI hỗ trợ trong bài Lab Day 18.

---

## 1. CÁC CÔNG CỤ AI ĐÃ SỬ DỤNG

- [ ] ChatGPT (OpenAI)
- [ ] Claude (Anthropic)
- [X] Google Gemini
- [X] Cursor / Antigravity Agent
- [ ] Khác: Không có

---

## 2. PHẠM VI ỨNG DỤNG AI TRONG BÀI LAB

### A. Gợi ý cơ chế tương tác và kịch bản (Mechanism Ideation)

- **Prompt đã hỏi AI:***"Dựa trên phát hiện người học thường xuyên bị kẹt lý thuyết slide và làm sai Quiz trên VLearn nhưng ngại chuyển tab ra ngoài hỏi ChatGPT, hãy gợi ý 4 cơ chế Human–AI interaction phân cấp theo mức độ can thiệp (Agency) từ thấp đến cao (User-initiated in-line, Co-creation diagnostic quiz, Proactive nudge, Human escalation with auto context)."*
- **AI đã gợi ý gì hữu ích:**AI đã đề xuất cấu trúc 4 cấp độ Agency tương ứng với Option A (In-line Inspector chạm vào đoạn kẹt), Option B (3-Question Diagnostic Quiz), Option C (Proactive Nudge sau thời gian dwell-time), và Option D (Human Handoff gom bối cảnh tự động gửi Mentor). AI cũng gợi ý việc dùng thang đo độ chắc chắn (Confidence level) để tăng tính minh bạch cho AI.
- **Phần tôi tự sàng lọc / thay đổi:**
  Tôi đã loại bỏ các đề xuất quá phức tạp của AI như "chat giọng nói (Voice agent)" hoặc "tự động sinh slide mới", đồng thời đưa ra yêu cầu khắt khe: toàn bộ tương tác của 4 options phải nằm trọn vẹn trong 1 màn hình học duy nhất, thời gian tương tác dưới 1 phút và có nút khôi phục quyền kiểm soát (như nút "Không đúng chỗ", "Làm lại", "Tắt tự nhắc").

### B. Sinh dữ liệu mẫu & Phản hồi mẫu (Synthetic Data & Canned Responses)

- **AI hỗ trợ tạo phần dữ liệu nào:**AI hỗ trợ sinh nội dung kiến thức mẫu cho 3 chủ đề AI/ML thực tế trên VLearn: *Context Window (Slide 12)*, *ReAct Agent (Slide 9)*, và *Gradient Descent (Slide 7)*; bao gồm nội dung tóm tắt, câu hỏi trắc nghiệm kiểm tra nhanh, và các câu hỏi vi mô (micro-quiz) chẩn đoán lỗ hổng cho Option B.
- **Mức độ can thiệp thực tế của tôi:**
  Tôi đã trực tiếp rà soát và điều chỉnh lại câu chữ tiếng Việt chuyên ngành, tinh chỉnh các phương án nhiễu (distractors) của câu hỏi quiz để sát với các lỗi sai thực tế mà học viên khóa trước hay mắc phải (ví dụ: hiểu nhầm 8.000 token là 8.000 từ, hoặc quên tính cả token input và output trong cùng một context window).

### C. Hỗ trợ kỹ thuật / Code giao diện (Prototype Coding / Design boilerplate)

- **AI đã hỗ trợ code hoặc dàn layout phần nào:**AI hỗ trợ dựng khung mã nguồn HTML/Vanilla CSS/JavaScript độc lập cho file [`prototype/index.html`](file:///c:/Users/Vxtor/Documents/workspace/ai20k/Track1_Day18_02495_LaiBaQuan/prototype/index.html): thiết kế hệ thống layout 2 cột (Slide bài giảng bên trái, Side panel trợ giảng bên phải), hiệu ứng viền vàng khi kích hoạt chế độ chọn đoạn kẹt của Option A, bộ đếm giờ tự động 12 giây cho Option C, và module ghi nhận nhật ký thao tác thời gian thực (Logger) kèm nút Copy dạng CSV.
- **Cách tôi chỉnh sửa để phù hợp với ngữ cảnh:**
  Tôi đã tinh chỉnh lại CSS để tuân thủ bảng màu chuẩn của VLearn (xanh navy đậm `#0f172a`, đỏ cam điểm nhấn `#ef4444`, và xanh dương AI `#2563eb`, tránh dùng gradient tím phổ biến của AI), viết lại logic gắn cờ `SS.tab` và `SS.opt` để đảm bảo chuyển đổi mượt mà giữa các hash URL mà không bị xung đột bộ nhớ log.

### D. Rà soát kịch bản phỏng vấn (Bias & Leading Question Check)

- **AI đã phát hiện những câu hỏi dẫn dắt nào trong kịch bản ban đầu:**AI phát hiện câu hỏi thử nghiệm ban đầu của tôi có tính định kiến: *"Bạn có thấy cách AI tự trượt thẻ ra ở Option C thông minh và tiện hơn cách tự click ở Option A không?"* — câu hỏi này vừa mớm sẵn tính từ khen ngợi ("thông minh", "tiện"), vừa so sánh áp đặt.
- **Cách viết lại trung tính sau khi chỉnh sửa:**
  Được viết lại hoàn toàn trung lập: *"Khi nhìn thấy thông tin này hiển thị trên màn hình, suy nghĩ đầu tiên xuất hiện trong đầu bạn là gì?"* và *"Trong 4 cách vừa trải nghiệm, cách nào phù hợp nhất với thói quen học tập của bạn? Bạn chấp nhận đánh đổi điều gì khi chọn cách đó?"*.

---

## 3. ĐÁNH GIÁ PHẢN BIỆN (CRITICAL REFLECTION VỀ AI)

- **Điểm yếu / Lỗ hổng lớn nhất trong các phản hồi của AI:**

  1. *Thiên vị giao diện lý tưởng (Happy Path Bias):* AI có xu hướng mặc định người dùng luôn đọc kỹ từng câu chữ và bấm đúng nút; AI không lường trước được rằng người học thật sự thường "lướt mắt qua rất nhanh", bấm nhầm khối, hoặc cuộn chuột bỏ qua thẻ giải thích để cắm đầu làm Quiz.
  2. *Thiếu tính thực tế về độ trễ (Latency Naivety):* AI thường đề xuất các luồng hội thoại dài 4-5 lượt chat mà không nhận ra rằng trong môi trường học tập áp lực cao (như ca lab 4 tiếng), người học chỉ kiên nhẫn tối đa 10–15 giây trước khi từ bỏ sang ChatGPT.
  3. *Ngôn ngữ mẫu (Canned copy) bị văn vở:* Lời thoại trợ giảng AI ban đầu do máy sinh ra quá dài dòng, mang tính xoa dịu khách sáo; tôi phải cắt bỏ hơn 60% từ ngữ thừa để đưa lời giải thích về dạng gạch đầu dòng ngắn gọn, đi thẳng vào bản chất công thức.
- **Bài học kinh nghiệm về việc kiểm soát AI trong quy trình Human–AI Design:**
  AI là một đối tác tạo mẫu nhanh (Prototyping Accelerator) cực kỳ xuất sắc trong việc sinh boilerplate code và khung sườn tương tác. Tuy nhiên, **quyền quyết định (Product Judgment) và tính chân thực của dữ liệu phải 100% thuộc về con người**. Nếu không trực tiếp ngồi quan sát người dùng thật bấm ngập ngừng ở đâu và lắng nghe họ than phiền điều gì, người làm sản phẩm rất dễ rơi vào ảo tưởng rằng một giao diện AI mượt mà trên lý thuyết sẽ tự động giải quyết được vấn đề thực tế của người học.
