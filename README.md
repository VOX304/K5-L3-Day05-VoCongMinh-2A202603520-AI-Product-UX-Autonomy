# TakingCare — LAB5 · T1 Y tế

Bài thực hành cá nhân lớp **L3A** về **trải nghiệm khi AI sai** và **mức tự chủ theo cái giá khi sai**. Hai màn hình mô phỏng một khách hỏi thuốc và dược sĩ nhận ca, không phải dịch vụ tư vấn y tế.

**Tác giả:** VoCongMinh · **Mã học viên:** 2A202603520 · **Bàn/zone:** cá nhân.

**Repo chính của bài làm:** [K5-L3-Day05-VoCongMinh-2A202603520-AI-Product-UX-Autonomy](https://github.com/VOX304/K5-L3-Day05-VoCongMinh-2A202603520-AI-Product-UX-Autonomy).

Bài được hoàn thiện ngay trong repo fork của tác giả, giữ lịch sử Git và tài liệu chương trình. `spec.md` và thư mục `prototype/` nằm ngay ở gốc. [README đề bài nguyên bản](docs/de-bai/README.md), các file hướng dẫn, `tracks/` và `prototype-sample/` vẫn được giữ để đối chiếu.

**Phân biệt nội dung và quy chế:** bản này dùng fork và làm cá nhân theo lựa chọn tác giả. README gốc yêu cầu repo mới, cách đặt tên khác và nhóm ba người; chưa có hướng dẫn riêng thay thế. Xem [checklist nộp bài](docs/checklist-nop-bai.md) để biết phần đã hoàn thành và phần còn cần giảng viên xác nhận.

## Mở bài

1. Mở [prototype/index.html](prototype/index.html) bằng Chrome hoặc Edge. Không cần cài đặt, API key, đăng nhập hay máy chủ.
2. Đọc [spec.md](spec.md) để đối chiếu từng yêu cầu và lý do chọn thiết kế.
3. Đọc [giải thích nguyên lý và flow](docs/learning-guide.md), rồi thực hành theo [kịch bản demo](docs/demo.md).

### Thử trong ba phút

- **S01:** xem “Không chờ trong chat” dù hồ sơ còn thiếu. Sang phía dược sĩ, tắt “Có người trực”; về phía khách, cảnh báo vẫn còn.
- **S02:** bấm “Bổ sung: Mình đang bầu 3 tháng” → gợi ý cũ thu hồi → chọn đã/chưa dùng → sang dược sĩ nhận ca. Nút duyệt thẻ vẫn bị chặn.
- **S03:** sang dược sĩ → nhận ca → duyệt → về khách mới thấy thẻ minh hoạ. Sửa thai kỳ làm thẻ và duyệt cũ mất hiệu lực.
- Thử quá hạn, huỷ chuyển trước lúc nhận, đồng ý lưu/xoá và tin tự do không có trong các ca dựng.

## Bài gồm gì?

| Tệp | Mục đích |
|---|---|
| [spec.md](spec.md) | 13 kịch bản, hai ca đắt nhất, UX khi sai, quyền của năm tool, nguyên tắc, tiêu chí và trạng thái demo |
| [prototype/](prototype/) | Bản mẫu hai màn hình, chạy ngay trên máy |
| [Hai ảnh đánh số](prototype/README.md) | Đối chiếu số chú thích với G2/G10/G9 |
| [docs/learning-guide.md](docs/learning-guide.md) | Giải thích cách đi từ rủi ro đến flow và cách tự bảo vệ lập luận |
| [docs/demo.md](docs/demo.md) | Bài nói 4 phút, ca để tự thử và câu hỏi kiểm tra hiểu |
| [docs/verification.md](docs/verification.md) | Kết quả chạy thật, phạm vi bằng chứng và phần chưa hoàn tất |
| [GLOSSARY.md](GLOSSARY.md) | Thuật ngữ thống nhất: người nhắn/người dùng thuốc, tự chủ, duyệt, thu hồi |
| [docs/adr/](docs/adr/) | Lý do giữ các ranh giới quan trọng của thiết kế |
| [tests/](tests/) | Kiểm tra logic và tương tác trình duyệt |
| [docs/checklist-nop-bai.md](docs/checklist-nop-bai.md) | Các yêu cầu đã có bằng chứng, khác biệt với đề gốc và bước nộp thực tế |
| [README đề nguyên bản](docs/de-bai/README.md) | Giữ đầy đủ hướng dẫn chương trình; các file đề và track ở gốc không bị thay đổi |

## Mức tự chủ đã chọn

| Hành động | Mức |
|---|---|
| Chuyển dược sĩ | Tự làm, có trạng thái thật trong mô phỏng và huỷ trước lúc nhận |
| Cảnh báo cần đi khám/cấp cứu | Tự làm, không đợi duyệt |
| Gửi gợi ý sản phẩm | Cần dược sĩ duyệt đúng thông tin và còn hạn |
| Lưu ghi chú sức khoẻ | Cần khách đồng ý riêng, rút lại/xoá được |
| Bán thuốc kê đơn | Cấm trong chat tự động |

**Quan trọng:** bản mẫu không có thuốc, liều hoặc danh mục sản phẩm thật. Thẻ minh hoạ chỉ dùng kiểm tra thứ tự duyệt/gửi. AI, dược sĩ và việc chuyển/lưu đều được mô phỏng; nội dung không gửi đi đâu. Thông tin chỉ nằm trong bộ nhớ trang và mất khi tải lại.

## Chạy kiểm tra — chỉ khi muốn kiểm tra mã

Cần Node.js. Kiểm tra logic không cần thư viện ngoài:

```text
npm test
```

Kiểm tra nút, hai màn hình, quyền lưu và tạo lại hai ảnh:

```text
npm ci --ignore-scripts --no-audit --no-fund
npm run test:browser
```

Trình kiểm tra dùng Chrome đã cài ở đường dẫn mặc định Windows. Máy khác đặt biến `CHROME_PATH` trỏ tới trình duyệt Chromium/Chrome tương thích. `playwright-core` chỉ phục vụ kiểm tra, không cần để mở prototype.

## Thông tin nộp bài

- **Repo đang dùng:** `K5-L3-Day05-VoCongMinh-2A202603520-AI-Product-UX-Autonomy`, giữ tên và quan hệ fork theo yêu cầu tác giả.
- **Truy cập:** repo công khai, fork từ `VinUni-AI20k/K5-L3-Day05-AI-Product-UX-Autonomy`; không thay đổi lịch sử đề để biến thành repo độc lập.
- **Cấu trúc bắt buộc:** [spec.md](spec.md) có bảng tác giả ở đầu; [prototype/](prototype/) có mã chạy được, hướng dẫn và [hai ảnh đánh số](prototype/README.md).
- **Cách chấm:** đọc `spec.md` §1–§7, đối chiếu ảnh và bấm các ca S01/S02/S03 trong prototype. [Bản đối chiếu bằng chứng](docs/verification.md) ghi kết quả kiểm tra và giới hạn.
- **Cách nộp:** tác giả gửi link repo qua kênh giảng viên thông báo. Cần được xác nhận việc dùng fork, tên repo và bài cá nhân nếu muốn khẳng định đáp ứng quy chế gốc. Việc push mã không đồng nghĩa đã nộp bài qua kênh lớp.
- **Hình thức:** cá nhân theo lựa chọn tác giả. Đề gốc yêu cầu ba người; chưa có ngoại lệ do giảng viên xác nhận, không tạo thêm thành viên hay tranh luận nhóm.
- **Demo/bonus:** chưa demo với TA/giảng viên và chưa có ca lạ từ người ngoài. Không có lời gọi AI thật; không nhận bonus cho các phần chưa thực hiện.
- **Thời hạn trong đề:** L3A — 23:59 ngày 12/11/2026. Lịch sử Git không thay thế bằng chứng đã gửi bài qua kênh lớp đúng hạn.

Đây là bài học thiết kế với bối cảnh Hỏi dược sĩ. Không liên kết với Pharmacity, không dùng dữ liệu sức khoẻ thật, không thay thế người có chuyên môn.
