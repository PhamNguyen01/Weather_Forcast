# Dự báo thời tiết

## Phân tích giao diện

Giao diện trang web Windy bao gồm các thành phần chính sau:

- Bản đồ
- Thanh công cụ phía trên
- Thanh công cụ bên trái
- Thanh thời gian dưới cùng
- Thông tin chi tiết
- Biểu tượng thêm lớp bản đồ
- Cài đặt
- Phần mở rộng

### Thiết kế giao diện

Để tạo giao diện trang web Windy, hãy làm theo các bước sau:

1. Tạo khung chứa chính để chứa tất cả các thành phần của trang web.
2. Tạo thanh công cụ phía trên với biểu tượng trang web ở góc trên bên trái, hộp tìm kiếm, tùy chọn chọn mô hình dự báo thời tiết, chọn ngôn ngữ và đăng nhập/đăng ký tài khoản ở góc trên bên phải.
3. Thêm bản đồ chiếm phần lớn giao diện trang web vào khung chứa chính.
4. Tạo thanh công cụ bên trái với các nút để chọn thông số thời tiết khác nhau như gió, mưa, mây, sóng, áp suất không khí, nhiệt độ, v.v.
5. Tạo thanh thời gian dưới cùng để hiển thị dự báo thời tiết theo thời gian, với thanh trượt để xem dự báo trong tương lai hoặc quá khứ và tùy chọn chọn đơn vị thời gian (giờ hoặc ngày).
6. Khi người dùng nhấp vào một điểm trên bản đồ, hiển thị một cửa sổ thông tin chi tiết với thông tin thời tiết cụ thể tại điểm đó, bao gồm nhiệt độ, gió, độ ẩm, áp suất không khí và các thông tin khác.
7. Thêm biểu tượng "+" ở góc dưới bên phải của màn hình để người dùng có thể thêm các lớp bản đồ, chức năng so sánh mô hình dự báo thời tiết khác nhau và truy cập các công cụ khác.
8. Tạo biểu tượng bánh răng ở góc dưới bên trái của màn hình để truy cập menu cài đặt, cho phép người dùng điều chỉnh các tùy chọn như đ


# API: "fed32be58df3a0bd09ff4c02c0da7443", "527afe48950c282cf057bbcd097c6aff", "c9c8e558cd1dad0583f2600da8c72b7e"

pip install mysql-connector-python
pip install Flask
pip install flask-cors

CREATE TABLE users (
  id INT(11) NOT NULL AUTO_INCREMENT,
  username VARCHAR(50) NOT NULL,
  password VARCHAR(255) NOT NULL,
  email VARCHAR(100) NOT NULL,
  PRIMARY KEY (id)
);
