# TakingCare — các việc cần làm để nộp bài

**Bài:** T1 Y tế · **Lớp:** L3A · **Tác giả:** VoCongMinh · **Mã:** 2A202603520 · **Bàn/zone:** cá nhân.

**Repo chính:** [fork của tác giả](https://github.com/VOX304/K5-L3-Day05-VoCongMinh-2A202603520-AI-Product-UX-Autonomy). Ngày 14/11/2026, tác giả chọn hoàn thiện bài trên fork này và xác nhận chưa có hướng dẫn riêng thay thế README gốc. Giữ repo fork không đồng nghĩa đã được chấp thuận ngoại lệ về quy chế nộp.

## Nội dung đã chuẩn bị và cách kiểm tra

| Mục | Bằng chứng | Trạng thái |
|---|---|---|
| Lát cắt, phạm vi T1 | `spec.md` §1, năm việc không làm và lý do | Đã có |
| Kịch bản rủi ro | 13 ca phủ bốn lớp, hai ca đắt nhất và ca suýt chọn ở §2 | Đã có |
| UX khi sai | Câu AI nguyên văn, màn hình, bước tiếp, ai nhận, phương án loại, loại lỗi ở §3 | Đã có |
| Mức tự chủ | Đủ năm tool, người duyệt, điều kiện/quá hạn và ba ca diễn tập ở §4 | Đã có |
| Prototype | `prototype/index.html`, hai màn hình; hai ảnh đánh số ở `prototype/evidence/` | Đã có, cần giữ khớp với bản code cuối |
| Nguyên tắc | G2/G10/G9 đối chiếu đúng vị trí ①–⑦ ở §5 | Đã có |
| Tiêu chí kiểm tra | P1/P2/P3, kết quả và giới hạn ở §6, `docs/verification.md` | Đã có |
| Giải thích và demo | `docs/learning-guide.md`, `docs/demo.md`, glossary và hai ADR | Đã chuẩn bị; không thay thế việc tác giả tự giải thích |
| Repo có bài ngay ở gốc | `README.md`, `spec.md`, `prototype/`, `tests/` cùng lịch sử fork | Đã push nhánh `main` và xác minh GitHub khớp bản local |
| Tài liệu chương trình | `docs/de-bai/README.md`; các file đề, `tracks/`, `prototype-sample/` ở gốc | Giữ nguyên để đối chiếu |

Ngày 14/11/2026 đã chạy lại **35 kiểm tra logic và 13 kiểm tra trình duyệt**, đều đạt. Đã xác minh repo đọc được không đăng nhập, vẫn là fork của chương trình và giữ đủ 12 tệp đề ban đầu (README gốc được lưu riêng). Chi tiết bằng chứng ở [verification.md](verification.md).

## Những điểm chưa thể ghi là đã đáp ứng quy chế gốc

| Vấn đề | README/đề gốc yêu cầu | Thực tế hiện tại | Việc cần xác nhận/làm tiếp |
|---|---|---|---|
| Loại repo | [README gốc](de-bai/README.md) §Nộp bài: repo mới, không fork | Repo chính là fork theo lựa chọn tác giả | Cần giảng viên xác nhận chấp nhận nộp fork, hoặc quyết định áp dụng đúng phương án repo mới của đề |
| Tên repo | `K5-<L3A/L3B>-Day05-<T1..T5>-<tên nhóm>` | Giữ tên `K5-L3-Day05-VoCongMinh-2A202603520-AI-Product-UX-Autonomy` | Xác nhận tên hiện tại được chấp nhận; không tự đổi tên repo tác giả |
| Nhóm | Đúng ba người, có mã học viên và việc mỗi người làm | Tác giả làm cá nhân; không có thành viên/trao đổi nhóm được tạo thêm | Xác nhận ngoại lệ cá nhân; chọn làm cá nhân trong chat chưa phải chấp thuận của giảng viên |
| Demo | Ca T1 trẻ nhỏ/nguy hiểm và một ca lạ do người xem đưa; giải thích phần mình làm | Có bản chạy và ca tự dựng; chưa demo với TA/giảng viên | Demo thật, ghi nguyên văn ca lạ và kết quả vào `spec.md` §7 sau khi diễn ra |
| Hạn/kênh | L3A: 23:59 ngày 12/11/2026, nộp link theo kênh thông báo trong lớp | Bài được làm/cập nhật 13–14/11; chưa có bằng chứng đã gửi bài | Xác nhận việc tiếp nhận bổ sung nếu cần và gửi link qua đúng kênh; không dùng ngày commit để tự nhận nộp đúng hạn |

Không tự chấm điểm thay giảng viên. Không nhận bonus demo lớp hoặc AI thật khi chưa thực hiện.

## Flow từ hoàn thiện mã đến nộp

1. Đọc `spec.md` và bấm S01/S02/S03; bảo đảm màn hình thể hiện đúng các quyết định.
2. Chạy kiểm tra, đối chiếu hai ảnh với bản code hiện tại và đọc giới hạn mô phỏng.
3. Commit/push vào đúng repo fork chính; mở trang chính thấy bài và liên kết đến tài liệu đề.
4. Kiểm tra repo công khai bằng truy cập không đăng nhập; kiểm tra mã trên GitHub khớp bản đã kiểm tra.
5. Đối chiếu các điểm khác quy chế ở bảng trên với giảng viên/chương trình.
6. Tác giả gửi link repo qua kênh lớp, lưu xác nhận nhận bài và hoàn thành demo. Push GitHub không tự thực hiện các bước này.

## Ghi nhận sau khi nộp/demo thật

- Kênh nộp và thời điểm: **chưa có**.
- Người/kênh xác nhận nhận bài: **chưa có**.
- Chấp thuận các khác biệt về fork/tên/cá nhân: **chưa có**.
- Ca lạ nhận ở demo và kết quả: **chưa có**, ghi tại `spec.md` §7 khi diễn ra.
