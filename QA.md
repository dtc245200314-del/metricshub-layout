# Kiểm tra thực tế ngày 19/10/2026

Đã kiểm tra trên trình duyệt ở viewport 1200×900, 768×900 và 375×844. Cả ba kích thước đều có scrollWidth bằng clientWidth, không tràn ngang. Bootstrap CSS tải thành công; ảnh SVG/ảnh sản phẩm tải được. Ảnh lazy trong CreativeChronicle tải sau khi cuộn đến phần Recommended.

Gallery: 4 cột desktop, 2 cột tablet, 1 cột điện thoại. CreativeChronicle: Recommended 4/2/1 cột; author và gallery đổi bố cục mobile. MetricsHub: pricing 3 cột từ 768px, 1 cột mobile; bento dùng span trên desktop và một cột mobile. Surface: menu mobile mở được, modal Compare hiển thị, FAQ mở nội dung; sau kiểm tra đã xóa viewport override. Login demo gửi form hợp lệ và xóa password; CreativeChronicle sao chép liên kết thành công. Hai JavaScript nội bộ qua node --check.

Sửa lỗi phát hiện: giảm gutter khối Design của Surface từ g-5 xuống g-4 để không tràn ngang điện thoại. Máy chủ preview được bổ sung MIME image/svg+xml để ảnh SVG hiển thị đúng. Không dùng bộ số đo trước sửa làm bằng chứng kết quả.