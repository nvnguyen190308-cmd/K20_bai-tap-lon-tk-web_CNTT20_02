## Thông tin sinh viên

- Họ và tên: Nguyễn Văn Nguyên 
- Mã sinh viên – Lớp:2071020144  – CNTT20_02
- Ngày thực hiện: 25/11/2026
- Link repository:https://github.com/nvnguyen190308-cmd/K20_bai-tap-lon-tk-web_CNTT20_02
- URL website: _(dán URL GitHub Pages sau khi deploy)_
- Tình huống: [x] Website của tôi (PawCare DNU – Dịch vụ Chăm sóc Động vật)

---

## 1. Nhận định của tôi trước khi hỏi AI

- **Vấn đề/yêu cầu**: Cần xây dựng website dịch vụ chăm sóc động vật bằng HTML5/CSS3 thuần cho môn FIT4014, bám sát cấu trúc mẫu báo cáo và bảng rubric A3.
- **Mong muốn và hiện tượng**: Muốn có giao diện rõ ràng, thân thiện, responsive tốt trên nhiều kích thước màn hình và đầy đủ các mục cần thiết mà không phụ thuộc framework CSS bên ngoài.
- **Dữ kiện đã kiểm tra**: Đọc tài liệu hướng dẫn A3, xem mẫu báo cáo và cấu trúc dự án web tĩnh, xác định các khu vực cần có (hero, danh mục dịch vụ chăm sóc động vật, bảng gói/quy trình, form đặt lịch, trang chi tiết và tài liệu bàn giao).
- **Tôi nghi nguyên nhân khó**: Phối hợp bố cục CSS Grid + Flexbox giữa nhiều thành phần (thẻ dịch vụ, bảng so sánh gói chăm sóc, biểu mẫu đặt lịch, thanh điều hướng) và giữ không tràn ngang ở màn hình hẹp dễ phát sinh lỗi nếu thiếu kế hoạch ngay từ đầu.
- **Vì sao**: Các khối nội dung có độ dài khác nhau và cần thích ứng mượt mà giữa màn hình rộng (`>= 992px`) và màn hình hẹp (`<= 768px`, đặc biệt `375px`).

---

## 2. Tôi hỏi AI và nhận được gợi ý

- **Nguồn**: [x] Công cụ AI: Gemini / Trợ lý AI hỗ trợ lập trình & tài liệu
- **Câu hỏi/prompt tôi đã gửi**:

  > "làm báo cáo bài tập lớn A3 và mã nguồn website tĩnh HTML5/CSS3 cho chủ đề Dịch vụ Chăm sóc Động vật (PawCare DNU) theo đúng mẫu FIT4014 và ghi nhận phần AI log"

- **Thông tin bổ sung tôi cung cấp** (khi rà soát và hoàn thiện):
  - Thông tin SV: Phạm Quốc Bảo, CNTT20_02
  - Tên dự án: PawCare DNU – Website Dịch vụ Chăm sóc Động vật (khám sức khỏe định kỳ, tiêm phòng – tẩy ký sinh trùng, spa/grooming, lưu trú chăm sóc & đặt lịch)
  - Cấu trúc dự án: `index.html`, `chi-tiet-dich-vu.html`, `css/style.css`, `images/*.svg`, `README.md`, `AI_LOG.md` và báo cáo A3
  - Định hướng giao diện: Bố cục phân tầng rõ ràng, tông xanh ngọc/xanh navy kết hợp cam ấm, HTML5 ngữ nghĩa + CSS3 thuần, đáp ứng rubric A3 (`A3.TC1a` – `A3.TC7`)

- **Gợi ý/kết quả của AI**:
  - AI đối chiếu yêu cầu `R1–R4` và các tiêu chí rubric A3 (`A3.TC1a` – `A3.TC7`) cho chủ đề dịch vụ chăm sóc động vật
  - AI sinh ra cấu trúc báo cáo A3, mã nguồn `index.html`, `chi-tiet-dich-vu.html`, `css/style.css`, hình minh họa SVG trong `images/`, `README.md` và phần nhật ký sử dụng AI
  - Áp dụng: Thẻ ngữ nghĩa HTML5, CSS Grid, Flexbox, biến màu `:root`, media queries responsive, HTML5 form validation và tài liệu bàn giao

---

## 3. Quyết định của tôi

- [ ] Chấp nhận kết quả AI sinh ra làm điểm khởi đầu
- [x] Chỉnh sửa thêm rồi áp dụng
- [ ] Bác bỏ


- **Lý do**: Nội dung bám sát cấu trúc mẫu A3 và yêu cầu `R1–R4` của chủ đề dịch vụ chăm sóc động vật, dùng HTML5/CSS3 thuần, có phân trang/neo điều hướng rõ ràng và biểu mẫu đặt lịch cơ bản; tuy nhiên cần trực tiếp kiểm tra giao diện trên trình duyệt, điền thông tin/commit thực tế và xác minh triển khai GitHub Pages.

---

## 4. Thực hiện và kiểm chứng

- **Tệp/vị trí đã tạo**:
  - `index.html` – Trang chính giới thiệu dịch vụ chăm sóc động vật, bảng gói tham khảo, quy trình 4 bước và form đặt lịch
  - `chi-tiet-dich-vu.html` – Trang chi tiết từng nhóm dịch vụ (`#kham`, `#tiem`, `#spa`, `#luu-tru`)
  - `css/style.css` – Toàn bộ stylesheet (biến màu, Grid/Flexbox, bảng, biểu mẫu và media queries)
  - `images/*.svg` – Hình minh họa cho 4 nhóm dịch vụ chăm sóc động vật
  - `README.md` – Hướng dẫn mở chạy và ghi nhận giới hạn website tĩnh
  - `AI_LOG.md` – Nhật ký sử dụng AI (file này)

- **Nội dung thay đổi sau khi nhận code từ AI**:
  - _(Điền các thay đổi bạn tự sửa thêm: cập nhật Mã SV, dán link repository/GitHub Pages và mã commit thực tế, thay/bổ sung ảnh minh họa hoặc chỉnh sửa nội dung gói dịch vụ nếu cần)_

| Nội dung kiểm tra | Trước xử lý | Sau xử lý |
|-------------------|-------------|-----------|
| Responsive trên mobile 375px | _(kiểm tra trên trình duyệt ở 375px)_ | _(điền kết quả thực tế)_ |
| Form validation (bỏ trống / nhập hợp lệ) | _(kiểm tra thao tác gửi form)_ | _(điền kết quả thực tế)_ |
| Điều hướng & tải CSS / ảnh SVG | _(kiểm tra liên kết & đường dẫn)_ | _(điền kết quả thực tế)_ |
| GitHub Pages hiển thị đúng phiên bản | _(kiểm tra sau khi push & deploy)_ | _(điền kết quả thực tế)_ |

- **Cách thử lại**: Mở dự án trong Visual Studio Code, chạy bằng Live Server hoặc mở trực tiếp `index.html` trên trình duyệt, mở DevTools kiểm tra ở các độ rộng `375px` / `768px` / `1440px`, thử gửi form đặt lịch và đối chiếu mã commit trên GitHub với trang GitHub Pages sau khi đẩy code.

---

## 5. Kết luận

- [ ] Đã xử lý được  [ ] Xử lý được một phần  [ ] Chưa xử lý được
- **Điều tôi rút ra**: _(Điền sau khi hoàn thành kiểm thử và deploy – ví dụ: cách tổ chức bố cục HTML5 ngữ nghĩa và CSS Grid/Flexbox responsive cho website dịch vụ, cách kiểm tra lỗi tràn ngang trên màn hình hẹp và quy trình xác minh phiên bản triển khai trên GitHub Pages)_
