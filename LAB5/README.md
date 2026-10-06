# LAB5 — Thiết lập mô hình tường lửa pfSense

## Thông tin sinh viên

- Họ và tên sinh viên: Trương Văn Quyết
- Mã số sinh viên: 1150080155
- Tên bài Lab: Thiết lập mô hình tường lửa pfSense
- Nội dung thực hiện: Xây dựng môi trường mạng ảo nội bộ gồm tường lửa pfSense bảo vệ vùng LAN và DMZ. Cấu hình các giao diện mạng (WAN, LAN, DMZ) và cài đặt các máy ảo kiểm thử bao gồm Windows Server (Domain Controller) và máy Ubuntu (LAN-Test). Trọng tâm bài thực hành tập trung giải quyết 3 tình huống cấu hình tường lửa cụ thể:
  1. **Tình huống 1:** Thiết lập luật chặn ping (ICMP) nhưng vẫn cho phép truy cập dịch vụ Web (TCP 80/443) và phân giải tên miền (TCP/UDP 53) cho toàn mạng LAN.
  2. **Tình huống 2:** Cấu hình cấp quyền truy cập Internet độc quyền cho một host cụ thể trong LAN (Domain Controller - `10.0.0.2`), đồng thời chặn (Block) toàn bộ các máy còn lại (như LAN-Test - `10.0.0.3`) đi ra Internet.
  3. **Tình huống 3:** Thiết lập rule cô lập vùng mạng DMZ, chặn hoàn toàn truy cập từ DMZ ngược vào mạng LAN để bảo vệ hệ thống nội bộ, nhưng vẫn duy trì kết nối ra Internet cho các máy chủ dịch vụ trong DMZ.
- Kết quả thực hiện: Qua bài LAB đã nắm vững quy trình triển khai và cấu hình tường lửa pfSense trong môi trường ảo hóa; hiểu rõ cơ chế hoạt động, thứ tự ưu tiên xử lý của các rule tường lửa (từ trên xuống dưới) và tính năng Outbound NAT. Vận dụng thành công các quy tắc để kiểm soát lưu lượng mạng ở mức độ giao thức (ICMP, TCP, UDP) và cổng dịch vụ. Đánh giá được tầm quan trọng của kiến trúc phân vùng mạng (tách biệt khu vực rủi ro cao DMZ khỏi mạng LAN cốt lõi). Qua 3 tình huống thực tế, chứng minh được hiệu lực của tường lửa trong việc ngăn chặn các truy cập trái phép, bảo vệ tài nguyên mạng, quản lý luồng dữ liệu một cách chặt chẽ và thu hẹp hiệu quả bề mặt tấn công.
