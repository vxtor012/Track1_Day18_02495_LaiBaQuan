# PROTOTYPE FEEDBACK NOTE (CÁ NHÂN)

> **Người thực hiện facilitate & ghi chép:** Lại Bá Quân (2A202602495)
> **Phương án phụ trách chính:** Option A (Chỉ vào chỗ kẹt - Inline Inspector & Contextual Help)
> **Quy định**: Phiên này do chính bạn trực tiếp điều phối độc lập với 1 tester ngoài nhóm. Tester được trải nghiệm ĐỦ CẢ 4 OPTIONS (A, B, C, D) trên cùng một chủ đề bài học và cùng một Outcome Task.

---

## 1. THÔNG TIN PHIÊN TEST

- **Tester (Tên viết tắt / Mã):** Tester 1 - `N.T.A (Học viên khóa 4 track 2 AI in Action )`
- **Bối cảnh thực tế (Relevant Context):** Từng nhiều lần gặp tình trạng khi gọi OpenAI API hoặc dùng chatbot với prompt dài thì model tự nhiên quên mất system prompt ban đầu. Khi học trên slide gặp công thức `context window >= token input + token output`, bạn thường bỏ qua và copy thẳng tài liệu vào ChatGPT nhờ tóm tắt lại thay vì ngồi tính toán số token.
- **Chủ đề test:** Context Window (Slide 12 · Lý thuyết) - URL: `prototype/index.html#context/theory/A`
- **Thời gian thực hiện:** 05/10/2026 · 20:15 – 20:40 (25 phút) · Trực tiếp 1-1 tại phòng tự học thư viện
- **Thứ tự trải nghiệm các options:** A ➔ B ➔ C ➔ D

---

## 2. BẢNG GHI NHẬN HÀNH VI (OBSERVATION LOG)

| Tiêu điểm quan sát                                                                                                                                       | Ghi nhận chi tiết trong lúc test                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **First Action** *(Hành động đầu tiên họ làm: đọc bài, bấm nút `Tôi vẫn chưa hiểu`, hay làm câu hỏi nhanh)*                    | Đọc lướt tiêu đề và công thức trong 15 giây đầu; vừa thấy nút*"Tôi vẫn chưa hiểu"* màu xanh dương ở góc phải bài là bấm ngay mà chưa đọc hết phần chữ bên dưới hay làm câu hỏi nhanh.                                                                                                                                                                                                                                                                                                                                                       |
| **Chỗ dừng, do dự hoặc hiểu sai** *(Điểm khựng lại, bấm nhầm, ngập ngừng)*                                                              | • Ở**Option A**: Khi các khối nội dung sáng viền vàng và thanh Pickbar hiện ra yêu cầu *"Chạm vào đoạn bạn chưa hiểu"*, tester khựng lại 11 giây phân vân không biết nên click vào dòng công thức hay đoạn văn bản giải thích token.• Ở **Option B**: Dừng lại khá lâu (~27 giây) ở câu hỏi trắc nghiệm số 2 vì câu hỏi có phép tính nhẩm token khiến tester phải đọc đi đọc lại.• Ở **Option D**: Tester ngập ngừng khi nhìn thấy danh sách các thẻ bối cảnh AI tự soạn gửi cho TA. |
| **Evidence & Uncertainty** *(Họ có đọc giải thích/căn cứ "Vì sao AI nghĩ vậy", trích dẫn nguồn, thước đo độ chắc chắn không?)* | • Có bấm vào link trích dẫn`Slide 12 · context window` ở thẻ Option A và gật đầu khi thấy slide nhảy hiệu ứng highlight.• Ở Option B, tester chú ý đến nhãn `Độ chắc chắn: Cao` và cụm mini-badge `[✓] [✗] [✓]`.• Ở Option C, tester mở mục *"Vì sao AI nghĩ vậy"* để xem tín hiệu thời gian dừng.                                                                                                                                                                                                                                |
| **Cách tester sửa sai hoặc lấy lại control** *(Nút Làm lại, Đóng ×, Bỏ qua, Tắt tự nhắc, Không đúng chỗ họ dùng thế nào?)*    | • Bấm nút*"Làm lại"* ở góc thanh Prototype Bar khi lỡ tay chọn nhầm sang đoạn khác.• Bấm nút *"Đóng ×"* trên thẻ in-line `icard` sau khi đã hiểu giải thích để giao diện trở về trạng thái gọn gàng ban đầu.• Ở Option D, tester chủ động bấm tắt chip *"Lịch sử làm sai"* trước khi gửi.                                                                                                                                                                                                                                     |
| **Option được chọn cuối cùng**                                                                                                                   | **Option A (Chỉ vào chỗ kẹt - In-line Inspector)**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Lý do lựa chọn & Trade-off** *(Họ thích điểm gì và chấp nhận đánh đổi điều gì?)*                                                 | •**Thích nhất**: Tốc độ phản hồi cực nhanh (<5 giây), giải thích hiện ngay tại chỗ bên dưới đoạn mình thắc mắc, không bị chuyển hướng sang giao diện khác hay bắt làm thêm quiz dài dòng.• **Trade-off chấp nhận**: Tester thừa nhận nếu bản thân gặp một bài học quá mới mà không biết mình "hổng ở đâu" thì sẽ lúng túng không biết nên bấm vào đoạn nào.                                                                                                                                            |
| **Evidence đi ngược lại kỳ vọng của nhóm** *(Điểm gì tester làm khiến nhóm bất ngờ?)*                                                | Nhóm từng kỳ vọng người học sẽ rất thích Option B vì có chẩn đoán phân loại lỗ hổng kiến thức khoa học và biểu đồ SVG; tuy nhiên tester nhận xét:*"Đang học mà bắt làm thêm 3 câu hỏi trắc nghiệm nữa thì hơi mệt đầu, mình chỉ muốn biết ngay công thức này tính thế nào để trả lời câu hỏi bên dưới thôi"*.                                                                                                                                                                                                        |

---

## 3. PHÂN TÍCH 4 LỚP DỮ LIỆU (FOUR-LAYER ANALYSIS)

### 1. OBSERVED (Dữ liệu quan sát khách quan)

*Dán dữ liệu nhật ký CSV trích xuất từ nút `Facilitator log` ➔ `Copy dạng CSV` của prototype vào đây:*

```csv
time,option,t_sec,event,detail
20:15:02,A,0,start,"bắt đầu bài học context/theory/A"
20:15:17,A,15,open-help,"mở chế độ chọn đoạn kẹt"
20:15:28,A,26,a-select,"chọn=[formula]"
20:15:32,A,30,a-help,"kiểu=simpler (Giải thích dễ hơn)"
20:15:34,A,32,a-send,"chọn=[formula] kiểu=simpler sửa_tay=false → formula"
20:15:48,A,46,cite,"Slide 12 · context window"
20:15:58,A,56,a-close,"đóng thẻ icard"
20:16:15,A,73,quick-question,"chọn đáp án 2 (Bản tóm tắt bị cắt giữa chừng - Đúng)"
20:16:45,B,0,start,"chuyển sang phương án B"
20:16:55,B,10,open-help,"mở trợ giảng chẩn đoán"
20:17:08,B,23,b-answer,"token=đúng"
20:17:35,B,50,b-answer,"budget=sai"
20:17:52,B,67,b-answer,"memory=đúng"
20:17:53,B,68,b-diag,"budget (Cao)"
20:18:20,B,95,reset,"làm lại để đổi phương án"
20:18:35,C,0,start,"chuyển sang phương án C"
20:18:48,C,13,c-nudge,"tự động sau 12s"
20:18:55,C,20,open-why,"vì sao AI nghĩ vậy"
20:19:12,C,37,c-accept,"budget"
20:19:40,D,0,start,"chuyển sang phương án D"
20:19:50,D,10,open-help,"mở modal hỗ trợ người thật"
20:20:05,D,25,d-toggle-context,"history=ẩn"
20:20:12,D,32,d-send,"tới=ta chia_sẻ=[topic,task,time] ghi_chú=không"
20:20:27,D,47,d-reply-arrived,"panel mở"
```

*Ghi lại chính xác những gì tester đã nói (nguyên văn quotes) và các thao tác thực tế họ đã click:*

- Hành động: Bấm vào nút *"Tôi vẫn chưa hiểu"* ➔ Click chọn khối công thức viền vàng ➔ Bấm chọn chip *"Giải thích dễ hơn"* ➔ Đọc lướt qua thẻ giải thích in-line ➔ Click vào link trích dẫn bài giảng ➔ Đóng thẻ và quay xuống làm đúng câu hỏi kiểm tra nhanh chỉ sau 15 giây.
- Lời nói / Câu hỏi của tester:
  > *"Bấm vào đoạn công thức này xong nó giải thích ngay ở dưới nhìn sướng mắt ghê, không phải mở tab ChatGPT mới rồi copy paste dài dòng."* (00:35)
  > *"Ủa cái này (Option B) phải trả lời tận 3 câu trắc nghiệm nữa hả bạn? Nếu mình đang vội làm bài lab thì chắc mình skip luôn qua Google tra cho nhanh."* (02:40)
  > *"Cái nút đóng thẻ này tiện, hiểu xong bấm tắt là trang web lại gọn gàng như cũ."* (01:10)
  >

### 2. INTERPRETED (Diễn giải ý nghĩa)

*Nhóm/bạn phỏng đoán hành vi trên thể hiện tâm lý hay trở ngại gì của người dùng:*

- **Tâm lý coi trọng tính tức thì (Immediacy Bias):** Người học khi bị kẹt kiến thức thường có tâm lý nóng vội muốn có câu trả lời trong vòng 5–10 giây. Bất kỳ rào cản nào (như phải làm bài quiz chẩn đoán 3 câu của Option B hay chờ đợi người thật 15 giây của Option D) đều kích hoạt phản xạ "muốn thoát ra ngoài tự tra ChatGPT".
- **Nhu cầu kiểm soát ngữ cảnh (Spatial Context Retention):** Việc giữ nguyên vị trí bài học và chèn câu trả lời in-line ngay dưới đoạn kẹt (Option A) giúp người học không bị mất dấu vị trí đang đọc trên slide, giảm tối đa chi phí tải nhận thức (Cognitive Load).
- **Rào cản tự chẩn đoán (Metacognition Barrier):** Tester mất 11 giây do dự khi chạm chọn khối vì không chắc chắn nguyên nhân mình không hiểu là do công thức toán hay do khái niệm token. Điều này chỉ ra rằng Option A cần có thêm gợi ý nhận diện thông minh khi người học chưa biết bắt đầu từ đâu.

### 3. DECIDED — NEXT CHANGE (Đề xuất thay đổi)

*Từ phát hiện của phiên này, bạn đề xuất nhóm nên sửa đổi, giữ lại hoặc loại bỏ chi tiết nào trong thiết kế:*

- **Giữ lại (Keep):** Giữ nguyên tương tác chạm khối viền vàng và hiển thị thẻ in-line card kèm trích dẫn nguồn của Option A vì đây là cơ chế được tester đánh giá cao nhất về tốc độ và tính trực quan.
- **Sửa đổi (Refine):**
  1. Khi người học làm sai câu hỏi nhanh (Quiz) ở cuối slide, tự động gắn cờ highlight nhẹ vào 1-2 khối liên quan trực tiếp đến đáp án sai để người học không bị lúng túng khi chọn đoạn kẹt.
  2. Rút gọn bộ câu hỏi chẩn đoán của Option B từ 3 câu xuống còn đúng **1 câu trắc nghiệm vi mô (~10s)** đặt ngay trong thẻ in-line của Option A khi người học chọn chế độ *"Ôn kiến thức nền"*.
- **Loại bỏ (Remove):** Loại bỏ tính năng tự động nhảy thẻ sau 12 giây của Option C (Auto-nudge) vì gây xao nhãng không cần thiết khi người học đang tập trung đọc bài.

### 4. STILL UNPROVEN (Điều vẫn chưa thể khẳng định)

*Nhận thức rõ giới hạn của 1 phiên test: Điều gì vẫn cần thêm dữ liệu để chứng minh?*

- Chưa kiểm chứng được khả năng chọn vùng kẹt của Option A trên các đoạn code dài 50-100 dòng trong các bài thực hành Lab (liệu việc chọn một dòng code có đủ để AI hiểu bối cảnh của toàn bộ hàm hay không).
- Chưa chứng minh được liệu người học hiểu nhanh nhờ in-line card có nhớ được lâu hay không, hay sẽ gặp lại lỗi tương tự ở các bài học tiếp theo.
