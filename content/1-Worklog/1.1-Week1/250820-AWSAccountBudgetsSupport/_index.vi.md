---
title: "AWS Account, Budgets và Support"
weight: 4
chapter: false
pre: " <b> 1.1.4 </b> "
---

### Tổng quan

Ghi chú này ghi lại buổi học về AWS Account, AWS Budgets và AWS Support để chuẩn bị môi trường học an toàn trước khi tạo tài nguyên.

### Nội dung đã học

* Xem quy trình đăng ký và quản lý AWS Account.
* Tìm hiểu trách nhiệm của root user và lý do cần bảo vệ account.
* Học cách AWS Budgets theo dõi chi phí và gửi cảnh báo.
* Xem cách truy cập AWS Support Center.
* Phân biệt support case về account, billing và technical.

Sau khi xem luồng tạo account, tôi ghi chú rằng root user có quyền rất cao và không nên dùng cho công việc hằng ngày. Account nên được bảo vệ trước, sau đó mới dùng IAM user hoặc role để làm lab.

Với AWS Budgets, tôi chưa triển khai ứng dụng gì nhưng vẫn cần hiểu cách đặt cảnh báo chi phí. Khi bắt đầu tạo EC2, VPC hoặc các dịch vụ khác, budget alert giúp phát hiện chi phí bất thường sớm hơn.

Tôi cũng xem qua luồng AWS Support để biết vị trí cần vào nếu gặp vấn đề về billing hoặc account access.

### Tài liệu đã xem

* Các lab AWS Study Group về AWS Account, AWS Budgets và AWS Support.
* AWS Cost Management documentation về tạo budget.
* Các trang AWS Console liên quan đến account, billing và support.

### Tổng kết

1. **Kiểm soát chi phí**: AWS Budgets quan trọng với account học tập.
2. **An toàn account**: Root user cần được bảo vệ và hạn chế sử dụng.
3. **Quy trình hỗ trợ**: AWS Support giúp xử lý vấn đề account hoặc billing.
