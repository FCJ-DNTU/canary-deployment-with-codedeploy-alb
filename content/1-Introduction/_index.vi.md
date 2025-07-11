+++
title = "Giới thiệu"
date = 2020-05-14T00:38:32+07:00
weight = 1
chapter = false
pre = "<b>1. </b>"
+++

**Canary Deployment** là một kỹ thuật triển khai ứng dụng giúp giảm thiểu rủi ro bằng cách chỉ triển khai phiên bản mới cho một phần nhỏ người dùng trước khi áp dụng cho toàn bộ hệ thống. Với sự phát triển của các hệ thống microservices và DevOps, Canary Deployment đã trở thành một phương pháp phổ biến để triển khai ứng dụng một cách an toàn và hiệu quả.

![Canary Deployment](/images/1-introduction/canary.png)

### Cách Canary Deployment hoạt động

1. **Triển khai phiên bản mới**: Triển khai phiên bản mới và chạy song song với phiên bản cũ.

2. **Chuyển lưu lượng nhỏ**: Chuyển một phần nhỏ lưu lượng truy cập (1-5%) sang phiên bản mới.

3. **Kiểm thử và giám sát**: Kiểm thử và giám sát phiên bản mới trong môi trường thực tế.

4. **Chuyển toàn bộ lưu lượng**: Nếu phiên bản mới hoạt động ổn định, chuyển toàn bộ lưu lượng sang phiên bản mới.

Canary Deployment có thể được thực hiện **2 bước** (two-step) hoặc **tuyến tính** (linear):

- **Two-step:** Triển khai phiên bản mới → cho nhóm nhỏ người dùng dùng thử → nếu đạt yêu cầu → mở rộng cho toàn bộ môi trường.

- **Linear:** Tăng traffic sang phiên bản mới theo từng đợt nhỏ cho đến khi tất cả người dùng sử dụng bản phát hành mới.

### Lý do áp dụng:

- **Giảm downtime:** Phát hiện lỗi sớm trên nhóm người dùng nhỏ.

- **Tự động rollback:** Nếu phát sinh lỗi, hệ thống tự động chuyển traffic trở lại phiên bản ổn định.

- **Quản lý traffic linh hoạt:** Điều phối traffic qua **Application Load Balancer (ALB)**.

- **A/B Testing:** So sánh song song hiệu suất các phiên bản.

- **Monitoring & Performance Analysis:** Theo dõi, thu thập số liệu và ra quyết định tự động.
