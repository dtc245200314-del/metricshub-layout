# Chiến lược dàn trang

Navbar cũ chia ba ô pixel cố định, nên tổng chiều rộng vượt điện thoại và từ tiếng Đức tràn ô. Flexbox mới phân phối không gian theo nội dung, canh giữa dọc, có gap và flex-wrap. Menu được đẩy thành hàng riêng dưới 768px, vẫn giữ thứ tự DOM và thứ tự bàn phím.

Dashboard là bài toán hai chiều: các widget nằm trực tiếp trong một grid ba cột. Widget doanh thu chiếm hai cột và hai hàng; nhóm tiến độ chiếm hai cột. Không còn wrapper column lồng nhiều lớp hay chiều cao cố định cho widget. Minmax(0,1fr) và min-width:0 cho phép nội dung co lại. Dưới 768px, grid chuyển một cột và bỏ span.

Pricing là ba thẻ cùng trọng số. Bootstrap row, g-4, col-12 col-md-4, card và h-100 đáp ứng yêu cầu mà không thêm media query cho giá. Flexbox trong widget vẫn hữu ích khi căn biểu đồ hoặc icon; Grid và Flexbox có thể kết hợp ở các cấp khác nhau.

Ma trận kiểm tra: 1200px → bento ba cột, giá ba cột; 768px → giữ bento và giá; 375px → dashboard và giá một cột, navbar tự ngắt hàng. Cần kiểm tra giao diện thực trước khi xác nhận QA.
