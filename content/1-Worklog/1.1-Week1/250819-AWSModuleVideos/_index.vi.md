---
title: "Ghi chú video module AWS"
weight: 3
chapter: false
pre: " <b> 1.1.3 </b> "
---

### Tổng quan

Ghi chú này tổng hợp phần chuẩn bị từ việc xem video học AWS và xem module Explore AWS Services trước khi làm lab.

### Nội dung đã xem

* AWS global infrastructure và khái niệm cloud cơ bản.
* Vai trò của các dịch vụ IAM, VPC, EC2, Budgets và Support.
* Lộ trình học FCJ và kết quả mong đợi trong Week 1.
* Tư duy bảo mật cơ bản khi sử dụng cloud account.

### Ghi chú học tập

Ngày này tôi chủ yếu xem video tổng quan và đọc trước các trang module trước khi thao tác trong AWS Console. Mục tiêu chưa phải là hoàn thành lab, mà là hiểu mỗi dịch vụ dùng để làm gì.

Điểm quan trọng tôi ghi lại là các dịch vụ AWS thường liên kết với nhau. IAM quản lý quyền truy cập, Budgets hỗ trợ kiểm soát chi phí, VPC là lớp mạng, còn EC2 chạy tài nguyên compute bên trong network đó. Vì vậy, trước khi làm hands-on, tôi cần nắm được vai trò cơ bản của từng dịch vụ.

### Câu hỏi chuẩn bị

* Sau khi tạo AWS Account thì nên làm gì với root user?
* Khi nào nên dùng IAM user thay vì root user?
* Vì sao nên tạo budget alert trước khi làm lab?
* Public subnet và private subnet khác nhau ở điểm nào?

### Tài liệu đã xem

* Các trang module trong AWS Study Group Cloud Journey.
* AWS official documentation về IAM, VPC và AWS Budgets.
* Video YouTube tổng quan về các dịch vụ AWS cơ bản.

### Tổng kết

1. **Chuẩn bị module**: Hiểu rõ hơn nội dung trước khi làm hands-on lab.
2. **Liên kết dịch vụ**: IAM, VPC và EC2 thường đi cùng nhau trong kiến trúc AWS.
3. **Trách nhiệm cloud**: Cần quan tâm bảo mật và chi phí ngay từ đầu.
