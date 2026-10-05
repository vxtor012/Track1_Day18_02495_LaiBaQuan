# THREE-OPTION DESIGN SHEET (BẢN LÀM VIỆC CHÍNH THỨC NHÓM 4 NGƯỜI)

> **Nhóm:** Tung Tung Tung Sahur  
> **Thành viên:** Lại Bá Quân (2A202602495), Đỗ Lê Việt Anh (2A202602491), Nguyễn Thị Minh Khánh (2A202602546), Nguyễn Quang Huy (2A202602421)  
> **Case Study:** AI Tutor: Diagnostic Refresher (Hỗ trợ người học vượt qua điểm nghẽn kiến thức trên VLearn)

---

## PHẦN 1: TỔNG HỢP EVIDENCE & CHỐT HYPOTHESIS PROBLEM (CHẶNG 1)

### 1. Bảng đối chiếu Evidence (Fact vs. Interpretation)
| Practice Note | Người dùng thực sự làm/nói gì? (Raw Fact / Quote) | Điều nhóm diễn giải / suy đoán (Interpretation) |
| :--- | :--- | :--- |
| **Note 1**<br>*Interviewer: Đỗ Lê Việt Anh*<br>*Interviewee: Học viên khóa 3 (Lab Coach)* | *"Nghe giảng các thầy cô thì hiểu nhưng mà có một số các lý thuyết thì nhìn slide đương nhiên nhìn lại mà nó viết tắt thì chắc chắn không hiểu"*. Người học mất 30p–1h tra AI/YouTube để học lại; cảm thấy nản. | Người học hiểu đại ý khi nghe giảng nhưng bị đứt mạch khi tự ôn vì **thuật ngữ viết tắt / khái niệm cô đọng** trên slide bài giảng. |
| **Note 2**<br>*Interviewer: Nguyễn Thị Minh Khánh*<br>*Interviewee: Lan (Học viên VLearn)* | Nhận ra mình chưa hiểu khi **làm Quiz và bị sai đáp án**. Người học khẳng định nếu công cụ hỗ trợ bắt chờ 3–5 phút thì sẽ **chuyển tab sang ChatGPT** vì quá lâu; mong muốn câu hỏi chẩn đoán bấm chọn nhanh dưới 1 phút. | **Thời điểm vàng kích hoạt (Trigger) là khi làm sai Quiz**. Người học yêu cầu độ trễ cực thấp (< 1 phút) và cơ chế chọn nhanh (1 chạm), không muốn gõ chữ dài. |
| **Note 3**<br>*Interviewer: Lại Bá Quân*<br>*Interviewee: Học viên tự học Cloud* | Người học bỏ qua video lý thuyết lướt, nhảy thẳng sang làm lab vì *"quay lại làm lab dễ hiểu hơn"*. Vừa gõ lab vừa mở ChatGPT hỏi *"cái này dùng để làm gì, có tác dụng gì"*. Thường xuyên không làm xong bài trong ca lab 4 tiếng trên lớp và phải mang về nhà. | Người học chuộng **Hands-on (học qua thực hành)**. Lý thuyết phải gắn liền với **tác dụng thực tế trong bài lab**, không chấp nhận lý thuyết hàn lâm suông. |
| **Note 4**<br>*Interviewer: Nguyễn Quang Huy*<br>*Interviewee: Học viên Khóa 3 (Nam)* | Người học chụp cả ảnh slide hoặc copy nguyên văn text ném vào ChatGPT. Nhận thức rằng AI trả lời sai ý là *"do con chat lan man và prompt của mình chưa clear"*. Chịu áp lực thời gian lớn vì phải học 2 buổi/ngày. | Người học **chưa biết cách đặt prompt chuẩn**, dẫn đến việc copy/paste máy móc vào AI ngoài và nhận lại câu trả lời lan man, làm trầm trọng thêm áp lực thời gian. |

### 2. Phát biểu Hypothesis Problem chuẩn của nhóm
- **Hypothesis Problem nhóm tiếp tục:**  
  *Học viên trên VLearn gặp bế tắc khi gặp các thuật ngữ viết tắt và khái niệm kỹ thuật trừu tượng trong lúc làm Quiz / thực hành Lab, dẫn đến việc bị đứt mạch học, mất 30–60 phút phải nhảy ra ngoài ném tài liệu vào ChatGPT (với prompt chưa chuẩn nên nhận về câu trả lời lan man), và thường xuyên không hoàn thành được bài học trong 4 tiếng trên lớp.*
- **Evidence ban đầu hỗ trợ giả thuyết:**  
  - 100% người học được phỏng vấn (4/4) đều sử dụng ChatGPT bên ngoài như một phương án chữa cháy bắt buộc khi không hiểu bài.
  - Hậu quả thực tế được ghi nhận từ 4 người học: Người học trong phiên của Việt Anh mất 30–60 phút tra cứu ngoài; người học trong phiên của Bá Quân thường xuyên không kịp nộp bài trong ca 4 tiếng; người học trong phiên của Quang Huy chịu áp lực lớn vì prompt chưa chuẩn nên AI trả lời lan man; và người học trong phiên của Minh Khánh khẳng định sẽ bỏ sang ChatGPT nếu công cụ bắt chờ quá 3 phút.
- **Điều quan trọng vẫn chưa được chứng minh:**  
  - Liệu việc hỗ trợ giải thích trực tiếp ngay tại ngữ cảnh bài học (In-context) có thực sự giúp người học hiểu bản chất và làm lab nhanh hơn, hay họ vẫn giữ phản xạ copy/paste sang ChatGPT ngoài?

---

## PHẦN 2: CHỌN BA SOLUTION OPTIONS (CHẶNG 2)

### 1. Những thứ BẮT BUỘC GIỮ NGUYÊN (70% Shared Core)
- **Target User:** Sinh viên / Học viên CNTT đang tự học trên nền tảng VLearn.
- **Situation:** Đang trong ca học 4 tiếng, đang giải một câu hỏi Quiz hoặc một bước thực hành Lab kỹ thuật Cloud.
- **Task:** Giải quyết câu hỏi trắc nghiệm / bước lab về chủ đề: *"Cấu hình mạng VPC và dải địa chỉ IP (CIDR Block)"*.
- **Desired Outcome:** Nắm bắt được ý nghĩa của thông số kỹ thuật trong vòng < 60 giây, chọn đúng đáp án Quiz và tự tin làm tiếp bài lab mà không cần mở tab khác.
- **Content/Data Fixture:**
  - Đề bài Quiz mẫu: *"Khi khởi tạo một VPC với dải địa chỉ CIDR `10.0.0.0/16`, phát biểu nào sau đây là ĐÚNG về số lượng IP khả dụng và vai trò của Subnet?"*
  - Điểm kẹt: Người học chọn sai đáp án do nhầm lẫn giữa khái niệm Subnet `/24` và VPC `/16`.

### 2. Bảng so sánh 3 Options (Comparison Contract)
| Tiêu chí | Option A: In-line Term Inspector | Option B: 30s Diagnostic Micro-Check | Option C: Proactive Context Action Card |
| :--- | :--- | :--- | :--- |
| **Solution Mechanism** | Tra cứu từ viết tắt / khái niệm tức thì tại chỗ qua hover/click vào từ khóa. | Chẩn đoán 2 câu trắc nghiệm 1-chạm để bóc tách chỗ hiểu sai trước khi giải thích. | AI chủ động phát hiện lỗi sai sau khi submit Quiz, tự động đẩy thẻ gợi ý sửa bài. |
| **User làm gì?** | Bôi đen hoặc click vào icon `[?]` cạnh từ khóa "CIDR Block" / "VPC". | Bấm nút "Chẩn đoán lỗi" ➔ Bấm chọn 2 câu trắc nghiệm nhanh ➔ Đọc giải thích. | Làm sai Quiz ➔ Đọc thẻ đề xuất tự động hiện lên ➔ Bấm "Thử lại" hoặc "Bỏ qua". |
| **AI làm gì?** | Hiển thị popover định nghĩa viết tắt + 1 ví dụ áp dụng thực tế ngắn gọn trong 1 dòng. | Đưa ra 2 câu hỏi phân loại nhận thức ➔ Phân tích lỗi tư duy ➔ Đưa tóm tắt trúng đích. | Phân tích đáp án sai của user ➔ Tự sinh thẻ Action Card chỉ ra điểm nhầm lẫn và gợi ý. |
| **Trigger kích hoạt** | **User click** có chủ đích vào từ khóa. | **User bấm nút** khi nhận kết quả Quiz sai. | **Hệ thống tự kích hoạt** ngay khi phát hiện nộp bài sai. |
| **Trade-off chính** | Cực nhanh (<5s), không đứt mạch; **Đánh đổi:** Giải thích ngắn, không kiểm tra được user đã thực sự hiểu sâu hay chưa. | Đánh trúng gốc rễ hiểu sai; **Đánh đổi:** Tốn thêm 30–45s thao tác chọn lựa của người học. | Tự động hóa cao, tiết kiệm công tìm kiếm; **Đánh đổi:** Dễ gây ức chế/mất tập trung nếu AI đoán sai ý định. |

### 3. Distance Check (Kiểm tra khoảng cách khác biệt)
- **A khác B vì:** Option A hoàn toàn do người dùng chủ động tra cứu thụ động từng từ ngữ (Lookup), trong khi Option B là cuộc đối thoại chẩn đoán hai chiều để bóc tách lỗ hổng nhận thức (Co-creation).
- **B khác C vì:** Option B yêu cầu người dùng chủ động kích hoạt và trả lời câu hỏi phân loại tư duy (AI Ask - User Decides), trong khi Option C là AI tự động nhảy ra can thiệp ngay khi thấy kết quả sai (AI Proactive Act - User Reviews).
- **A khác C vì:** Option A chỉ cung cấp thông tin tra cứu vi mô tại chỗ không phán xét, trong khi Option C chủ động phân tích hành vi sai và đưa ra phương án hành động cụ thể.

---

## PHẦN 3: HUMAN–AI DESIGN PASS (CHẶNG 3)

### Human–AI Decision Table
| Tiêu chí thiết kế | Option A: In-line Term Inspector | Option B: 30s Diagnostic Micro-Check | Option C: Proactive Context Action Card |
| :--- | :--- | :--- | :--- |
| **1. Role & Agency** | - User: Chủ động chọn từ cần tra cứu.<br>- AI: Đóng vai trò từ điển ngữ cảnh mini. | - User: Cung cấp tín hiệu suy nghĩ qua 2 câu chọn.<br>- AI: Đóng vai trò bác sĩ chẩn đoán tri thức. | - User: Duyệt hoặc bác bỏ gợi ý của AI.<br>- AI: Đóng vai trò trợ lý chủ động nhắc bài. |
| **2. AI Autonomy** | **Don't Act**: Không bao giờ tự động hiện nếu user không click. | **Ask**: AI đề xuất câu hỏi chẩn đoán và chờ user chọn đáp án. | **Act**: AI tự động đẩy thẻ phân tích lỗi ra màn hình ngay khi submit sai. |
| **3. Expectation** | Tooltip ghi rõ: *"Click để xem giải thích nhanh thuật ngữ trong bài lab"*. | Banner ghi rõ: *"Chẩn đoán nhanh trong 30 giây để tìm lý do bạn chọn chưa đúng"*. | Thẻ ghi rõ: *"Gợi ý tự động từ AI dựa trên câu trả lời vừa chọn của bạn"*. |
| **4. Evidence & Uncertainty** | Trích xuất trực tiếp từ Glossary chính thức của bài học; không suy đoán. | Hiển thị tag: *"Dựa trên 2 câu trả lời chẩn đoán của bạn"*; nếu phân vân sẽ gợi ý 2 hướng. | Hiển thị tag: *"Độ tin cậy: 85% - Có thể bạn đang nhầm Subnet với VPC"*. |
| **5. Control & Recovery** | Click ra ngoài hoặc bấm `[x]` để đóng popover ngay lập tức; không lưu vết. | Có nút *"Bỏ qua chẩn đoán / Xem giải thích chung"* để thoát ngay lập tức nếu không muốn chọn. | Có nút *"Bỏ qua (Dismiss)"* để tắt thẻ, hoặc nút *"Báo lỗi / Gợi ý sai"* để hệ thống ẩn đi. |
