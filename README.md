# Lab 21 — Phân tích rủi ro AI qua case study thực tế

- Họ và tên: Nguyễn Ngọc Linh
- MSSV / mã học viên: 2A202602480
- Lớp: K4 - Track 1
- Ngành đã chọn: News - AI trong tin tức (Media / news / social / political assistant)

### 1. Industry Risk Snapshot

| Nội dung | Đánh giá của tôi và lý do |
| --- | --- |
| Những tác hại chính có thể xảy ra | Lan truyền thông tin sai lệch, sai kiến thức chuyên sâu (tài chính, y tế, bầu cử), đạo văn/trùng lặp bản quyền, xúc phạm nhân vật hoặc định hướng dư luận sai. Người bị ảnh hưởng trực tiếp là độc giả (đưa ra quyết định sai lầm, thiệt hại tài chính), nhà báo/phóng viên (tổn hại uy tín nghề nghiệp, nguy cơ cắt giảm nhân sự), và cơ quan báo chí (mất niềm tin công chúng, khủng hoảng truyền thông, rủi ro pháp lý). |
| Mức độ high-stakes | Cao. Báo chí là nguồn thông tin chính thống định hình nhận thức cộng đồng với quy mô tiếp cận từ hàng chục nghìn đến hàng triệu người. Khi sai sót xảy ra trong các chủ đề nhạy cảm như tư vấn tài chính, sức khỏe, hay chính trị xã hội, tác hại xảy ra ngay lập tức và diện rộng, việc đính chính sau đó rất khó thu hồi hoặc bù đắp hoàn toàn niềm tin đã mất. |
| Dữ liệu nhạy cảm có thể được sử dụng | Danh tính người cung cấp tin ẩn danh / người tố giác (whistleblower), thông tin đời tư cá nhân chưa công bố (nạn nhân, trẻ vị thành niên, người bị nghi vấn), tài liệu mật/tài liệu cấm tiết lộ trước thời hạn (embargoed materials), và dữ liệu hồ sơ hành vi, khuynh hướng chính trị của độc giả. |
| Nhu cầu human review | Cao. Bắt buộc cần có Trưởng ban biên tập / Biên tập viên chuyên môn và kiểm chứng viên (fact-checker) duyệt bài ở bước tiền xuất bản (pre-publication gatekeeping). Lý do: Mô hình AI dễ sinh ảo giác (hallucination), không có ý thức đạo đức báo chí, không hiểu bối cảnh nhạy cảm địa phương và không thể chịu trách nhiệm pháp lý trước tòa án khi xảy ra kiện tụng vu khống/sai sự thật. |

### 2. Case study 1 — CNET & Red Ventures: Sự cố công cụ AI viết bài tài chính cá nhân sai lệch (2022–2023)

#### Brief Case

- Tổ chức / sản phẩm AI: Trang tin công nghệ & tiêu dùng CNET (thuộc tập đoàn truyền thông Red Ventures) sử dụng công cụ AI nội bộ thử nghiệm (CNET AI Engine).
- Thời gian, địa điểm / bối cảnh: Tháng 11/2022 – Tháng 01/2023 tại Hoa Kỳ. Trong xu hướng các cơ quan truyền thông tìm cách ứng dụng Generative AI để tăng năng suất sản xuất nội dung và tối ưu hóa thứ hạng tìm kiếm (SEO) nhằm thu hút tiếp thị liên kết (affiliate).
- AI được dùng để làm gì: Tự động tạo toàn bộ bài viết giải thích kiến thức tài chính cá nhân (financial explainers) như cách tính lãi kép (compound interest), chứng chỉ tiền gửi (CD), tỷ lệ phần trăm lợi tức hàng năm (APY) và các khoản vay thế chấp dưới bút danh chung "CNET Money Staff".
- Vấn đề hoặc sự kiện đáng chú ý: Chuyên trang công nghệ Futurism phát hiện và phanh phui việc CNET âm thầm đăng tải các bài viết tài chính do AI tạo ra mà không thông báo rõ ràng cho độc giả. Kiểm tra sâu hơn phát hiện các bài viết chứa lỗi tính toán toán học và định nghĩa tài chính cơ bản sai lệch nghiêm trọng, kèm theo nghi vấn đạo văn khi câu cú trùng lặp sâu với bài viết của Forbes Advisor. CNET đã phải tạm dừng công cụ và thực hiện rà soát, sửa đổi hàng loạt.
- Số liệu có nguồn: Theo cuộc rà soát nội bộ do CNET công bố và được The Verge tổng hợp ngày 25/01/2023, trong tổng số **77** bài viết do AI tạo ra được xuất bản, có tới **41** bài (chiếm **53,2%**, hơn một nửa) chứa các lỗi sai sự thật nghiêm trọng đòi hỏi phải đính chính toàn diện; toàn bộ dự án thử nghiệm AI viết bài tự động của CNET bị tạm dừng vô thời hạn.
- Nguồn:
  - Futurism (Maggie Harrison, Christian Peake — 16/01/2023): *"CNET Is Reviewing All Its AI-Written Articles After Finding Major Errors"* — URL: https://futurism.com/the-byte/cnet-reviewing-ai-articles
  - The Verge (James Vincent — 25/01/2023): *"CNET found errors in more than half of its AI-written stories"* — URL: https://www.theverge.com/2023/1/25/23571082/cnet-ai-written-stories-errors-corrections-red-ventures
  - CNET Statement (Connie Guglielmo, Tổng biên tập — 25/01/2023): *"CNET Is Pausing AI-Generated Stories After Finding Errors"* — URL: https://www.cnet.com/tech/cnet-is-pausing-ai-generated-stories-after-finding-errors/
- Phân biệt bằng chứng và nhận định:
  - Điều nguồn xác nhận: CNET thừa nhận chính thức 41 trên tổng số 77 bài viết (53,2%) bị sai thông tin và cần biên tập đính chính; xác nhận có lỗi tính sai lãi kép và một số đoạn tương đồng cấu trúc với bài báo khác; CNET đã dừng xuất bản bài viết bằng AI.
  - Điều tôi suy luận hoặc còn chưa rõ: Nguồn chưa đo lường được có bao nhiêu độc giả đã thực sự chịu thiệt hại tài chính khi làm theo những hướng dẫn sai trong 41 bài viết này; tôi suy luận áp lực tối đa hóa lưu lượng truy cập SEO và kiếm tiền affiliate từ tập đoàn mẹ Red Ventures đã khiến quy trình kiểm duyệt của con người bị cắt xén dẫn tới thất bại.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | [Tình huống cụ thể có rủi ro] |
| Stakeholder bị ảnh hưởng | [Người dùng và các bên liên quan] |
| Failure mode | [Kiểu lỗi AI] |
| Layer bắt đầu lỗi | [UX / Grounding / Safety / Model; giải thích hoặc ghi chưa đủ bằng chứng] |
| Harm xảy ra là gì? | [Ai bị ảnh hưởng + hậu quả; ghi rõ đã xảy ra hay mới là nguy cơ] |
| Harm lens | [Loại tác hại] |
| Severity | [Low / Medium / High / Critical] |
| Scale | [Quy mô tác động và căn cứ] |
| Probability | [Khả năng xảy ra và căn cứ] |
| Frequency | [Tần suất và căn cứ] |
| Vì sao? | [Lý do cho các đánh giá; nguồn hoặc giới hạn bằng chứng] |

### 3. Case study 2 — Gannett & LedeAI: Thất bại tự động hóa bản tin thể thao học đường (2023)

#### Brief Case

- Tổ chức / sản phẩm AI: Tập đoàn truyền thông Gannett (sở hữu mạng lưới báo chí USA Today Network và hơn 200 nhật báo địa phương tại Mỹ) hợp tác với công ty công nghệ LedeAI.
- Thời gian, địa điểm / bối cảnh: Tháng 8/2023 tại bang Ohio và nhiều địa phương tại Mỹ, vào dịp khởi tranh mùa giải bóng bầu dục các trường trung học phổ thông (high school football).
- AI được dùng để làm gì: Tự động chuyển đổi dữ liệu tỷ số thể thao thô thành các bài viết tổng thuật tin nhanh (game recaps) cho các tờ báo địa phương như *The Columbus Dispatch*, *Louisville Courier Journal*.
- Vấn đề hoặc sự kiện đáng chú ý: Hệ thống AI xuất bản hàng loạt bài báo có câu từ ngớ ngẩn, máy móc lặp đi lặp lại (ví dụ miêu tả trận đấu là "a close encounter of the athletic kind", bảng điểm "ngủ đông ở hiệp bốn"), thiếu tên cầu thủ và điểm nhấn chuyên môn; đặc biệt có bài xuất bản sót nguyên vẹn các mã biến giữ chỗ (placeholder code) dạng `[[WINNING_TEAM_MASCOT]]` và `[[LOSING_TEAM_MASCOT]]`. Sự việc bị độc giả phát hiện và chế giễu rầm rộ trên mạng xã hội, buộc tòa soạn phải gỡ bài, sửa đổi và tạm dừng công cụ.
- Số liệu có nguồn: Theo tường thuật của The Washington Post và CNN Business ngày 30/08/2023, Gannett đã phải tuyên bố dừng ngay lập tức việc dùng công cụ AI của LedeAI trên toàn bộ mạng lưới hơn **200** tờ báo địa phương; hàng chục bài viết đã xuất bản phải gắn dòng đính chính (Editor's Note) để biên tập lại thủ công; các bài viết lỗi thu hút hàng triệu lượt xem và bình luận chỉ trích trên mạng xã hội X.
- Nguồn:
  - The Washington Post (Will Oremus — 30/08/2023): *"A newspaper chain paused its AI tool after bizarre sports articles"* — URL: https://www.washingtonpost.com/technology/2023/08/30/gannett-ai-sports-articles-columbus-dispatch/
  - CNN Business (Oliver Darcy — 30/08/2023): *"Gannett pauses AI sports writing tool after readers mock awkward stories"* — URL: https://edition.cnn.com/2023/08/30/media/gannett-ai-sports-articles/index.html
  - The Guardian (31/08/2023): *"Newspaper publisher Gannett pauses AI bot after botched high school sports articles"* — URL: https://www.theguardian.com/media/2023/aug/31/gannett-ai-sports-articles-botched-ledeai
- Phân biệt bằng chứng và nhận định:
  - Điều nguồn xác nhận: Bài viết chứa lỗi placeholder kỹ thuật và văn phong máy móc kỳ dị đã thực sự được xuất bản công khai trên *The Columbus Dispatch*; phát ngôn viên của Gannett chính thức xác nhận việc tạm dừng hệ thống LedeAI trên các ấn phẩm toàn chuỗi.
  - Điều tôi suy luận hoặc còn chưa rõ: Nguồn chưa công bố con số chính xác có bao nhiêu bài báo tổng cộng đã được LedeAI tự động tạo trước khi dừng; tôi suy luận việc vội vã đưa AI thay thế phóng viên thể thao địa phương xuất phát từ việc cắt giảm nhân sự tòa soạn, nhưng quy trình hoàn toàn thiếu khâu kiểm duyệt trước khi đăng bài (zero human review) đã dẫn đến khủng hoảng uy tín thương hiệu nghiêm trọng.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | [Điền] |
| Stakeholder bị ảnh hưởng | [Điền] |
| Failure mode | [Điền] |
| Layer bắt đầu lỗi | [Điền] |
| Harm xảy ra là gì? | [Điền; phân biệt hậu quả đã xảy ra với nguy cơ] |
| Harm lens | [Điền] |
| Severity | [Điền] |
| Scale | [Điền] |
| Probability | [Điền] |
| Frequency | [Điền] |
| Vì sao? | [Điền căn cứ và giới hạn bằng chứng] |
