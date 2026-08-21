---
title: "Ghi chú học Amazon VPC"
weight: 6
chapter: false
pre: " <b> 1.1.6 </b> "
---

### Tổng quan

Amazon Virtual Private Cloud (Amazon VPC) dùng để tạo môi trường mạng riêng biệt trong AWS. Hôm nay tôi tập trung học quy trình làm VPC và vai trò của từng thành phần mạng trước khi triển khai đầy đủ.

### Nội dung đã học

* VPC và cách chọn CIDR block.
* Public subnet và private subnet.
* Route table và routing rule.
* Internet Gateway cho truy cập internet.
* Security Group như firewall ở cấp instance.
* Mối liên hệ cơ bản giữa VPC networking và EC2.

### Kế hoạch thực hành

* Tạo VPC với CIDR block phù hợp.
* Tạo subnet theo availability zone.
* Gắn Internet Gateway.
* Cấu hình route table cho public subnet.
* Kiểm tra Security Group trước khi launch EC2.

### Tổng kết

1. **Nền tảng VPC**: VPC là lớp mạng cơ bản cho nhiều workload AWS.
2. **Thiết kế subnet**: Public và private subnet giúp tách tài nguyên theo mức truy cập.
3. **Luồng routing**: Truy cập internet cần route table và Internet Gateway đúng.
