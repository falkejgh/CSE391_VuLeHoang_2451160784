Phần A

Câu A1

Ý 1 (nguồn tham chiếu: tuan_1_html5/01_introduction_html_universe.md + Cuộc Hành Trình 0.3 Giây Xuyên Đại Dương)

1. Request xuất phát từ laptop -> đi qua router WiFi nhà trọ
2. -> Qua hạ tầng của VNPT -> đi đường cáp quang biển
3. -> Đến Data Center của Shopee ở Jurong, Singapore . Khoảng cách: ~2.800 km.
4. -> Server xử lý: "Mình muốn xem danh sách đồ trong Giỏ hàng"
5. -> Response chạy ngược lại: cáp quang -> VNPT -> router -> laptop
6. -> Chrome nhận file HTML, CSS, JS -> render ra giao diện -> Mình thấy đôi giày mình định mua hiện ra trong giỏ hàng.

Ý 2 (nguồn tham chiếu: tuan_1_html5/01_introduction_html_universe.md + 4.3.Developer Tools (F12) — "Kính hiển vi" cho website)

- Tab network dùng để xem requests/responses
  ![alt text](./screenshot/screenshot.png)

Câu A2 (nguồn tham chiếu: tuan_1_html5/04_visible_part_html.md + Bản đồ Semantic Elements)

Trang web bị đánh giá thấp là bởi vì nó không có cấu trúc Semantic Elements

Các lỗi sai

1. Sai: Dùng <div> cho header
<div class="header">  sửa lại thành <header>
2. Sai: Menu không dùng <nav>
<div class="menu"> sửa lại thành <nav>
3. Sai: Nội dung chính dùng <div>
<div class="main"> sửa lại thành <main>
4. Sai: Sản phẩm không dùng <article>
<div class="product"> sửa lại thành <article class="product">
5. Sai: Footer dùng <div>
<div class="footer"> sửa lại thành <footer>
6. Sai: Ảnh không có alt
   <img src="iphone.jpg"> sửa lại thành <img src="iphone.jpg" alt="iPhone 16 Pro">

Câu A3 (nguồn tham chiếu: tuan_1_html5/04_visible_part_html.md + Block vs Inline — Hai loại element cơ bản)

Kết quả hiển thị:
Hộp 1
Text A Text B
Hộp 2
Text C Text D(có in đậm)
Hộp 3

Giải thích:
do Hộp 1, Hộp 2, Hộp 3 dùng thẻ <div> nên nó sẽ chiếm cả 1 dòng
thẻ Text A, Text B dùng thẻ <span> nên chỉ chiếm nội dung
thẻ Text C, Text D cũng giống Text A, Text B nhưng Text D có dùng thẻ <strong> nên in đậm

Câu A4 (nguồn tham chiếu tuan_1_html5/05_tables_hyperlinks.md + Table — Bảng dữ liệu)

so sánh sự khác nhau giữa <thead>, <tbody>, <tfoot>

<thead>	, vai trò: Header	,  Ghi nhớ: Tiêu đề cột
<tbody> , vai trò: Body	,  Ghi nhớ: dữ liệu chính
<tfoot> , vai trò: Header	,  Ghi nhớ: Tổng kết

Tại sao KHÔNG NÊN dùng table để tạo layout trang web? (Ghi rõ ít nhất 3 lý do)

1. Sai mục đích sử dụng (semantic sai)

- <table> được thiết kế để hiển thị dữ liệu dạng bảng (tabular data) như: bảng giá, thống kê, danh sách...
- Layout trang web (header, menu, sidebar…) không phải dữ liệu dạng bảng

2. Sai cấu trúc trang

- Khi dùng <table> để layout, các thành phần như header, nav, main không được phân tách rõ ràng
- Google không hiểu đâu là nội dung chính, đâu là điều hướng

3. Khó mở rộng code

- Code trở nên rối, khó đọc và khó sửa

Phần B
Bài B3:
Lỗi 1: Dòng 1 — <!DOCTYPE> sai cú pháp — Sửa thành <!DOCTYPE html>

Lỗi 2: Dòng 2 — Thiếu thuộc tính lang — Sửa thành <html lang="vi">

Lỗi 3: Dòng 4 — Thẻ <title> không đóng — Thêm </title>

Lỗi 4: Dòng 5 — charset viết sai (utf8) — Sửa thành UTF-8

Lỗi 5: Dòng 9 — Thẻ <h1> không đóng đúng — Sửa </h1>

Lỗi 6: Dòng 13 — Thẻ <a> không đóng — Sửa </a>

Lỗi 7: Dòng 20 — img thiếu dấu "" và thiếu alt — Sửa src="iphone.jpg" và thêm alt

Lỗi 8: Dòng 22 — Thẻ <b> đóng sai vị trí — Đưa </b> vào trước </p>

Lỗi 9: Dòng 27 — Bảng dùng <td> cho header — Sửa thành <th>

Lỗi 10: Dòng 36 — Dùng 2 thẻ <main> — Sửa thẻ thứ 2 thành <aside>

Lỗi 11: Dòng 41 — Thẻ <p> trong footer không đóng — Thêm </p>

Lỗi 12: DÒng 8 & 12 - Nhảy cấp trực tiếp từ <h1> -> <h3> - sửa h3->h2
