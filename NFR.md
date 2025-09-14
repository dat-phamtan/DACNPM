Mỗi NFR bạn viết nên có 3 thành phần:

Tên yêu cầu

Mô tả (nói rõ vì sao cần)

Thang đo (measurable metrics) — cái này quan trọng nhất để tránh mơ hồ.

⚡ Group 1 — Performance (Hiệu năng)

Mô tả hệ thống cần nhanh, đáp ứng tốt khi tải tăng

Một số yêu cầu gợi ý:

ID	Tên yêu cầu	Mô tả	Thang đo
P1	Response Time	Thời gian hệ thống trả kết quả cho người dùng phải nhanh để đảm bảo trải nghiệm tốt	≤ 2 giây cho 95% request
P2	Throughput	Hệ thống phải xử lý được nhiều yêu cầu đồng thời	≥ 100 request/giây
P3	Resource Utilization	Hệ thống không được sử dụng quá nhiều CPU/RAM	CPU < 70%, RAM < 80% khi tải cao
P4	Scalability	Hệ thống có thể mở rộng khi số lượng người dùng tăng	Thêm server mới giúp tăng throughput gần tuyến tính (≥80% hiệu quả)
🛡️ Group 2 — Reliability (Độ tin cậy)

Mô tả hệ thống phải ổn định, không hỏng, không mất dữ liệu

Một số yêu cầu gợi ý:

ID	Tên yêu cầu	Mô tả	Thang đo
R1	Uptime	Hệ thống luôn sẵn sàng hoạt động	≥ 99.5% uptime/tháng
R2	Fault Tolerance	Hệ thống vẫn hoạt động khi 1 thành phần bị lỗi	Không downtime khi 1 node server hỏng
R3	Data Integrity	Dữ liệu không bị lỗi, mất hoặc trùng lặp	0% lỗi dữ liệu trong quá trình xử lý
R4	Recovery Time	Thời gian khôi phục sau sự cố	< 15 phút để khôi phục dịch vụ
📌 Gợi ý khi viết báo cáo

Viết ngắn gọn, liệt kê các NFR theo bảng như trên để dễ đọc.

Luôn đưa ra con số đo được (thang đo): phần này giúp biến yêu cầu từ “mơ hồ” thành “có thể kiểm thử”.

Không đưa mục tiêu chung chung như “phải nhanh” hay “phải ổn định” — vì không đo được.
