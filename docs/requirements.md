# Mục tiêu và ma trận yêu cầu LAB5

## Những điều đã xác nhận

- Người học muốn hoàn thành bài thực hành, sau đó hiểu cách giải, nguyên lý và luồng xử lý.
- Track được chọn: **T1 — Y tế**; lớp **L3A**; thực hiện **cá nhân** (người dùng xác nhận trong chat).
- Người dùng chốt tên **TakingCare**, bàn/zone **cá nhân**, đồng ý để agent tự quyết chi tiết theo hai ca S01 trẻ có dấu hiệu nguy hiểm và S02 bổ sung thai kỳ sau gợi ý sai. Tác giả/mã giữ nguyên dạng `VoCongMinh` / `2A202603520` trong tên repo được cung cấp, không tự suy đoán dấu.
- Ngày 14/11/2026, người dùng xác nhận repo fork hiện tại là repo chính, giữ lịch sử và tài liệu đề; không có hướng dẫn riêng của chương trình/giảng viên thay thế README gốc.
- Yêu cầu gốc về nhóm đúng ba người không phù hợp cách làm cá nhân đã chọn. Không tạo danh tính, phân công, ý kiến tranh luận hay lịch sử demo giả để lấp chỗ trống.
- Đề yêu cầu chọn **một track**, không cần làm năm bài nộp.
- Chuẩn gốc yêu cầu repo mới, không fork. Quyết định làm việc hiện tại là hoàn thiện ngay trên fork theo yêu cầu tác giả; đây là khác biệt cần ghi rõ, không tự nhận đã được giảng viên cho phép.

## Tiêu chí hoàn thành có bằng chứng

| Mã | Yêu cầu | Bằng chứng cần có | Nguồn |
|---|---|---|---|
| R1.1 | Giữ nguyên lát cắt T1 | `spec.md` §1 và hành vi prototype | T1 / Lát cắt; rubric R1 |
| R1.2 | Ít nhất ba việc ngoài phạm vi, có lý do | `spec.md` §1; không có hành động trái phạm vi | rubric R1 |
| R2.1 | Ít nhất tám kịch bản phủ bốn lớp | Bảng kịch bản có mã, tin nhắn, lớp, lỗi dự kiến, ứng xử và mức hại | brief / Nghiệm thu; rubric R2 |
| R2.2 | Mỗi lỗi dự kiến có căn cứ cụ thể | Trỏ tới tool, dữ liệu hoặc dữ liệu còn thiếu trong T1 | rubric R2 |
| R2.3 | Chọn hai ca đắt nhất và một ca suýt chọn | So sánh hậu quả, khả năng khắc phục và lý do chọn/loại | rubric R2 |
| R3.1 | Hai ca chính có câu AI nói nguyên văn | `spec.md` §3 khớp với prototype | rubric R3 |
| R3.2 | Màn hình, bước tiếp theo, ai nhận, khi nào | Luồng khách và người nhận xử lý có trạng thái rõ | rubric R3 |
| R3.3 | Chọn hỏi lại / trả lời có giới hạn / chuyển người | Phân tích phương án được chọn và bị loại | rubric R3 |
| R3.4 | Hai đến ba nguyên tắc HAX/PAIR có vị trí cụ thể | Ảnh chú thích đánh số, bảng đối chiếu nguyên tắc | rubric R3/R5 |
| R3.5 | Phân loại lỗi hệ thống / người dùng / ngữ cảnh | Giải thích cách nhận trách nhiệm và sửa theo từng loại | rubric R3 |
| R3.6 | Một lỗi không thể cứu bằng câu chữ | Thay đổi quyền hành động, thu hồi hoặc bước xác nhận trong thiết kế | rubric R3 |
| R4.1 | Phân mức cho cả năm tool T1 | Bảng tự làm / cần duyệt / cấm | rubric R4 |
| R4.2 | Lý do theo hậu quả, đảo lại, thời gian chờ | Mỗi tool có phân tích riêng | rubric R4 |
| R4.3 | Tool cần duyệt có người duyệt, thông tin, quá hạn | Chính sách và hành vi prototype khớp nhau | guide §4; spec §4 |
| R4.4 | Tool khó xếp nhất và lựa chọn khác | So sánh phương án; ghi rõ phân tích cá nhân thay cho tranh luận nhóm | rubric R4; ngoại lệ cá nhân |
| R4.5 | Thử hai ca chính và một ca bình thường | Bảng diễn tập: chặn lỗi, còn làm quá quyền, có chờ vô ích | rubric R4 |
| R4.6 | Một mức tự chủ đổi lời hứa sản phẩm | So sánh lời hứa trước và sau | rubric R4 |
| R5.1 | Một đến hai màn hình bấm hết ca khó | Bản chạy được và kiểm tra tương tác từ đầu đến cuối | guide §5; rubric R5 |
| R5.2 | Thấy căn cứ hoặc giới hạn | Vị trí cụ thể trên màn hình, có ảnh | rubric R5 |
| R5.3 | Ít nhất hai mức tự chủ; tự làm có đường sửa | Kiểm tra xác nhận, thu hồi, chuyển người; không có nút thực hiện việc cấm | guide M3; rubric R5 |
| R5.4 | Ghi rõ phần mô phỏng, có hay không AI thật | `prototype/README.md` và `spec.md` §5 | spec §5 |
| R6.1 | Ba tiêu chí Pass/Fail chấm được | `spec.md` §6 | rubric R6 |
| R6.2 | Chấm thử hai ca chính, ghi giới hạn còn lại | Kết quả kiểm tra thực tế có thể đối chiếu | rubric R6 |
| R7.1 | Demo ca khó và ca lạ | Kịch bản diễn tập và kết quả thật; ca do người ngoài đưa phải ghi đúng nguồn | rubric R7 |
| R7.2 | Giải thích được phần việc của mình | Hướng dẫn trình bày và câu hỏi tự kiểm; việc người học đã hiểu cần người học xác nhận | README / Vibe-coding |
| S1 | Người dùng thuốc có thể khác người nhắn | Sàng lọc đúng người sẽ dùng; trẻ nhỏ, thai kỳ, người già và nhóm rủi ro được chuyển dược sĩ | T1 / Rubric riêng |
| S2 | Dấu hiệu nguy hiểm không nằm trong hàng chờ | Hiện hành động khẩn ngay; không đợi đủ hồ sơ, duyệt hoặc đồng ý lưu | T1 / Rubric riêng |
| S3 | Không liều, không bán thuốc kê đơn, không thay thế thuốc kê đơn | Nội dung và điều khiển trong toàn bộ prototype | T1 / An toàn |
| S4 | Không lưu sức khoẻ khi chưa đồng ý | Mặc định không lưu; quyền đồng ý rõ ràng, có cách rút lại/xoá | T1 / An toàn |
| S5 | Dữ liệu tình huống dựng | Nhãn dữ liệu dựng và không tích hợp tài khoản/nghiệp vụ thật | README / Luật chung |
| N1 | Định dạng bài nộp | `spec.md`, `prototype/`, một đến hai ảnh chú thích | README / Nộp bài |
| N2 | Danh tính thật của người học, lớp, mã | Người dùng xác nhận; không suy ra tên có dấu từ tên thư mục | README / Thành viên |
| N3 | Repo GitHub mới, công khai, đúng tên | URL và kiểm tra đọc khi chưa đăng nhập | README / Nộp bài |

## Phần không thể thay bằng dữ liệu dựng

- Nhóm ba người, phân công thật và phát biểu của từng thành viên: thực tế là bài cá nhân theo lựa chọn tác giả; chưa có ngoại lệ của giảng viên và không tự nhận đã đáp ứng yêu cầu nhóm.
- Ca lạ từ TA/giảng viên và demo trước lớp: có thể chuẩn bị và diễn tập nhưng chỉ được ghi đã diễn ra khi thực sự diễn ra.
- Học viên hiểu và tự giải thích được: có thể hỗ trợ bằng tài liệu, câu hỏi và đối thoại; không tự xác nhận thay học viên.
- Bonus gọi AI thật: chỉ được ghi có khi có lời gọi thật kèm bằng chứng. Bản mô phỏng không đủ điều kiện này.
- Repo công khai: phải kiểm tra trạng thái GitHub thực tế; file local hoặc zip không thay thế được URL.
- Hạn L3A trong đề là 23:59 ngày 12/11/2026. Không ghi đã nộp đúng hạn khi không có bằng chứng.

## Những điểm tài liệu chưa nhất quán

- Guide §3 có một chỗ dùng "cảm nhận"; spec và rubric dùng "ngữ cảnh". Dùng "ngữ cảnh" theo mô tả khái niệm và rubric.
- README nói "100 + 8"; rubric ghi tổng cuối không vượt 100. Không tự hứa điểm lớn hơn 100.
- README và rubric diễn đạt khác nhau về phạm vi 0 điểm khi không giải thích được. Chuẩn bị giải thích toàn bộ phần làm, không suy đoán quyền chấm điểm của giảng viên.

## Trạng thái làm việc

- Bộ bài TakingCare được đưa vào gốc repo fork: `spec.md`, `prototype/`, `tests/`, glossary và tài liệu học trong `docs/`. README đề nguyên bản được giữ riêng; tài liệu đề và lịch sử Git được bảo toàn.
- Đã push nhánh `main` vào repo fork chính và xác minh công khai không đăng nhập ngày 14/11/2026; mã trên GitHub khớp bản local, đủ 35 kiểm tra logic và 13 kiểm tra trình duyệt đạt. Chi tiết tại `docs/verification.md`.
- Tên tác giả/mã giữ nguyên dạng trong tên repo do người học cung cấp; tên bài và bàn/zone đã được xác nhận riêng.
- Các bản cũ trong `submission/` và `exports/` chỉ còn là bản lưu cục bộ, được loại khỏi nội dung commit của fork. Repo TakingCare riêng trước đó không được đổi tên, xoá hay dùng thay repo chính.
- Khác biệt với chuẩn gốc: loại repo fork, tên repo và hình thức cá nhân. Người dùng xác nhận chưa có hướng dẫn riêng cho phép các khác biệt này. Xem `docs/checklist-nop-bai.md`.
- Chưa nộp link cho giảng viên, chưa có demo với TA/giảng viên; bài không tự nhận điều đó đã diễn ra.
