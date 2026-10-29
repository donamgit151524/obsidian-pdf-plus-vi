# PDF++ — bản Việt hóa cá nhân

Phiên bản: 0.40.31-vi.1. Bản nền: PDF++ 0.40.31.

## Công dụng

PDF++ giúp đọc và ghi chú PDF ngay trong Obsidian:

- Sao chép liên kết đến đúng đoạn văn bản, trang hoặc vùng hình chữ nhật trong PDF rồi dán vào ghi chú.
- Tô sáng các đoạn PDF được ghi chú tham chiếu; có thể lần từ tài liệu sang ghi chú qua liên kết ngược.
- Nhúng một vùng PDF vào ghi chú, hữu ích với sơ đồ, công thức và hình minh họa.
- Tùy chọn ghi chú thích trực tiếp vào PDF; thêm, chèn, xóa, trích xuất hoặc tách trang khi bật chỉnh sửa.
- Tự chuyển sang ghi chú sau khi chép liên kết hoặc tự dán liên kết vào ghi chú đích.
- Cải thiện bảng màu, mục lục, ảnh thu nhỏ, tìm kiếm và phím điều khiển Vim.

## Cách dùng nhanh: đọc tài liệu và ghi chú

1. Đưa một PDF có lớp văn bản vào vault rồi mở trong Obsidian. PDF chỉ có ảnh scan cần OCR bằng công cụ khác trước khi chọn được chữ.
2. Mở một ghi chú Markdown cạnh PDF, chẳng hạn `Ghi chú tài liệu.md`.
3. Bôi chọn một đoạn trong PDF. Bấm màu trên bảng màu hoặc dùng lệnh **PDF++: Sao chép liên kết đến vùng chọn hoặc chú thích** trong khay lệnh (`Ctrl+P` trên Windows).
4. Dán vào ghi chú (`Ctrl+V`), rồi viết nhận xét của bạn bên dưới.
5. Bấm liên kết vừa dán để quay lại đúng đoạn PDF. Đoạn được tham chiếu có thể hiện màu theo cài đặt **Tô sáng liên kết ngược**.

Ví dụ: chọn đoạn mô tả HSE trong datasheet STM32, sao chép liên kết vào ghi chú RCC, rồi viết giải thích bằng lời của bạn. PDF++ giữ liên kết về nguồn để tra lại.

### Nhúng hình, bảng hoặc công thức

1. Chạy **PDF++: Bắt đầu chọn vùng chữ nhật** khi đang xem PDF.
2. Chọn vùng cần trích; sao chép và dán liên kết nhúng vào ghi chú theo thao tác của trình xem.
3. Trong cài đặt **Nhúng vùng chọn chữ nhật**, có thể bật **Dán dưới dạng ảnh** nếu muốn lưu ảnh tĩnh; nếu để liên kết nhúng, vùng được hiển thị từ PDF gốc.

### Tự chuyển tiêu điểm và tự dán

- **Tự chuyển tiêu điểm:** sau khi sao chép liên kết PDF, chuyển sang ghi chú đích để bạn tự dán.
- **Tự dán:** dán liên kết ngay vào ghi chú đích; cấu hình tệp đích và cách xác định tệp trước khi bật.
- Hai chế độ trên không bật đồng thời. Nên thử quy trình sao chép/dán thủ công trước, sau đó bật chế độ phù hợp.

### Ghi chú thích trực tiếp vào PDF

Vào cài đặt PDF++ → **Chỉnh sửa tệp PDF** → **Cho phép chỉnh sửa PDF**. Điền **Tác giả chú thích**, sau đó dùng nút ghi tô sáng vào tệp trên thanh công cụ PDF. Chú thích ghi vào tệp có thể được trình đọc PDF khác hiển thị, tùy loại chú thích được hỗ trợ.

Tô sáng dựa trên liên kết ngược và ghi tô sáng vào PDF là hai cơ chế khác nhau. Nếu chưa bật chỉnh sửa, việc liên kết từ ghi chú không tự ghi chú thích vào tệp gốc. Sao lưu PDF trước các thao tác sửa, xóa hoặc tách trang; bản gốc không hỗ trợ sửa PDF mã hóa.

## Cài bằng BRAT

1. Cài và bật **BRAT** từ Community plugins của Obsidian.
2. Vào BRAT → **Add beta plugin**.
3. Nhập `donamgit151524/obsidian-pdf-plus-vi` hoặc URL repository này.
4. Chọn bản mới nhất nếu có danh sách phiên bản, rồi **Add plugin**. Kiểm tra **Enable after installing the plugin** nếu muốn bật ngay.
5. Mở Settings → PDF++ để xem giao diện Việt hóa. Đóng/mở lại PDF hoặc tải lại plugin nếu giao diện cũ vẫn còn.

ID vẫn là `pdf-plus`, dùng chung với plugin gốc. Không cài hai bản cùng ID song song. Khi chuyển bản trên vault đang dùng, sao lưu `.obsidian/plugins/pdf-plus/data.json` trước; không cần chép cấu hình cá nhân lên GitHub. Cập nhật từ danh mục Community plugins có thể thay lại mã gốc; dùng BRAT để theo dõi bản Việt hóa này.

## Phạm vi Việt hóa

Việt hóa 495 vị trí giao diện tĩnh: tên/mô tả cài đặt, các đề mục chính, tên lệnh, nút và trình đơn thao tác. Giữ nguyên ID, khóa cài đặt, cú pháp mẫu, chuỗi có biến, tên sản phẩm và liên kết tài liệu. Một số hướng dẫn Markdown/HTML dài, thông báo động và tài liệu ngoài vẫn bằng tiếng Anh; đây không phải bản dịch toàn bộ tài liệu PDF++.

## Nguồn, giấy phép và phát triển tiếp

- Bản nền: [RyotaUshio/obsidian-pdf-plus 0.40.31](https://github.com/RyotaUshio/obsidian-pdf-plus/releases/tag/0.40.31), tác giả Ryota Ushio; giữ giấy phép MIT trong `LICENSE`.
- [Tài liệu chính thức](https://ryotaushio.github.io/obsidian-pdf-plus/) giải thích chi tiết các tính năng. Đây là bản tùy chỉnh cá nhân, không phải bản phát hành của tác giả gốc.
- `source-bundle.zip` chứa mã nguồn upstream đúng phiên bản, bản diff và từ điển/công cụ Việt hóa. Giải nén để xem `source/` và `patch-tools/`.
- Để áp dụng lại cho bundle gốc đúng phiên bản: đặt `apply.cjs` cạnh `vi.txt`, rồi chạy `node apply.cjs /duong-dan/main.js`. Công cụ sao lưu bundle trước khi sửa và kiểm tra cú pháp, ID lệnh, chuỗi mẫu có biến. Không chạy lại trên một bản đã dịch.
- Khi phát hành bản mới: cập nhật `main.js`, tăng `version` trong `manifest.json`, cập nhật `versions.json` và gói nguồn. Workflow GitHub Actions tạo release theo phiên bản, đính kèm `main.js`, `manifest.json`, `styles.css` và `source-bundle.zip` để BRAT tải được. Một phiên bản đã phát hành không bị ghi đè tự động.

Không bao gồm `data.json`, ghi chú hay thông tin đăng nhập của người dùng.

