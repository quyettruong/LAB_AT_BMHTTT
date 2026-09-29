# LAB4 — Khảo sát và đánh giá bề mặt mạng bằng Nmap

## Thông tin sinh viên

- Họ và tên sinh viên: Trương Văn Quyết
- Mã số sinh viên: 1150080155
- Tên bài Lab: Khảo sát và đánh giá bề mặt mạng bằng Nmap
- Nội dung thực hiện: Xây dựng môi trường mạng ảo nội bộ (Host-Only) gồm máy quét Kali Linux và máy mục tiêu Metasploitable 2. Cài đặt và sử dụng Nmap để rà soát phát hiện các host đang hoạt động; tiến hành khảo sát các cổng TCP/UDP bằng nhiều kỹ thuật chuyên sâu (TCP Connect, SYN, FIN, Xmas, NULL, ACK scan). Thực hiện dò tìm nhận diện phiên bản dịch vụ (`-sV`), fingerprinting hệ điều hành (`-O`, `-A`) và sử dụng Nmap Scripting Engine (NSE) để thu thập thông tin SMB, kiểm tra lỗ hổng MS17-010. Xuất kết quả quét ra các định dạng chuẩn (Normal Text, XML, Grepable, HTML). Cuối cùng, thực hiện tình huống gia cố hệ thống (Hardening) bằng tường lửa iptables để chặn cổng FTP và thu thập tệp bằng chứng trạng thái Before/After.
- Kết quả thực hiện: Qua bài LAB đã nắm vững quy trình lập bản đồ bề mặt mạng; hiểu rõ cơ chế tương tác của các cờ TCP/IP và phân biệt được ý nghĩa của các trạng thái cổng (open, closed, filtered, unfiltered). Đánh giá được mức độ rủi ro an ninh thông qua việc nhận diện chính xác các phần mềm, dịch vụ lỗi thời đang lắng nghe trên mục tiêu; vận dụng thành công script NSE để tự động hóa dò quét lỗ hổng bảo mật. Tổng hợp thành công hồ sơ bằng chứng an toàn mạng đa định dạng. Đặc biệt, thông qua kịch bản Hardening, chứng minh được hiệu lực của biện pháp phòng thủ bằng tường lửa khi chuyển đổi thành công trạng thái cổng từ phơi bày (open) sang vô hiệu hóa tiếp cận (filtered), giúp thu hẹp hiệu quả bề mặt tấn công mạng.
