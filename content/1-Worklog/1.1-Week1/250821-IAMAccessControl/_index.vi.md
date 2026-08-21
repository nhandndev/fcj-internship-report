---
title: "AWS IAM Access Control"
weight: 5
chapter: false
pre: " <b> 1.1.5 </b> "
---

### Tổng quan

AWS Identity and Access Management (IAM) là dịch vụ quản lý định danh và phân quyền trong AWS. Trong lab này, tôi thực hành tạo IAM user, group, role và switch role để hiểu cách kiểm soát truy cập an toàn.

### Nội dung lab

1. Introduction to IAM.
2. Create IAM Group and IAM User.
3. Create IAM Role and IAM User.
4. Switch Role.
5. Clean up resources.

### Nội dung đã hoàn thành

* Tạo IAM Group để tổ chức user.
* Tạo IAM User và cấp quyền thông qua group.
* Tạo IAM Role cho truy cập có kiểm soát.
* Thực hành Switch Role trong AWS Management Console.
* Dọn dẹp tài nguyên sau khi hoàn thành lab.

### Ghi chú lab

Tôi bắt đầu bằng phần giới thiệu IAM để phân biệt user, group, policy và role. Sau đó tôi làm theo từng bước trong AWS Console.

Phần user và group giúp tôi hiểu cách quản lý quyền gọn hơn. Thay vì gắn permission trực tiếp cho từng user, có thể đưa user vào group rồi quản lý permission ở group đó.

Phần role là nội dung hữu ích nhất trong lab. Tôi hiểu rằng role không phải là một user đăng nhập bình thường. Role dùng khi cần quyền tạm thời, còn Switch Role giúp đổi ngữ cảnh quyền mà không cần chia sẻ credential dài hạn.

### Tài liệu đã xem

* Lab AWS Study Group về IAM Access Control.
* AWS IAM documentation về policies và roles.
* AWS Management Console trong quá trình thực hành.

### Tổng kết

1. **IAM Group và User**: Group giúp quản lý quyền dễ và nhất quán hơn.
2. **IAM Role**: Role phù hợp cho truy cập tạm thời và có kiểm soát.
3. **Least privilege**: Chỉ nên cấp đúng quyền cần thiết cho từng nhiệm vụ.
