# LAB3 — Nhận diện và ứng phó các mối đe dọa đến an toàn thông tin

## Thông tin sinh viên

- Họ và tên sinh viên: Trương Văn Quyết
- Mã số sinh viên: 1150080155
- Tên bài Lab: Nhận diện và ứng phó các mối đe dọa đến an toàn thông tin
- Nội dung thực hiện: Xây dựng môi trường Windows 11 cho LAB3, cài đặt và sử dụng Microsoft Defender, Windows Event Log, Sysmon, Autoruns, Process Explorer, Wireshark và Python để thu thập bằng chứng và phân tích các mối đe dọa trên endpoint và mạng. Thực hiện baseline hệ thống; lập Risk Register theo mối quan hệ Asset → Vulnerability → Threat → Risk → Control; kiểm chứng khả năng phát hiện EICAR của Microsoft Defender; phân tích các sự kiện xác thực 4624, 4625 và 4648; nhận diện persistence và tiến trình lắng nghe cục bộ; quan sát lưu lượng HTTP/HTTPS; phân tích DoS, DDoS và Mail Bombing bằng dữ liệu thử nghiệm; nhận diện Social Engineering, Phishing và Spear Phishing; cuối cùng thực hiện cleanup, kiểm tra lại trạng thái hệ thống và tính SHA-256 cho các tệp bằng chứng.
- Kết quả thực hiện: Qua bài LAB có thể nhận diện và phân loại các nhóm mối đe dọa gồm hành động vô ý, hành động cố ý, thảm họa tự nhiên, lỗi kỹ thuật và lỗi quản lý; quan sát được khả năng phát hiện/quarantine của Microsoft Defender đối với tệp kiểm thử EICAR; sử dụng Windows Security Log để phân tích đăng nhập thành công và thất bại; sử dụng Sysmon, Autoruns và Process Explorer để tương quan dấu vết persistence và tiến trình; so sánh sự khác nhau giữa lưu lượng HTTP đọc được và HTTPS được mã hóa; phân tích tải cục bộ, dataset DDoS, log Mail Bombing và các mẫu Social Engineering/Phishing. Sau khi thu thập đủ bằng chứng, các artefact thử nghiệm được loại bỏ, endpoint protection vẫn hoạt động và các tệp Evidence được kiểm tra tính toàn vẹn bằng SHA-256.
