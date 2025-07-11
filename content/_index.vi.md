+++
title = "Canary Deployment với CodeDeploy và Application Load Balancer"
date = 2025
weight = 1
chapter = false
+++

# Canary deployment với CodeDeploy và Application Load Balancer

### Tổng quan

Trong workshop này, bạn sẽ:

- Hiểu được cách hoạt động và lợi ích của **Canary Deployment** trong môi trường production.

- Biết cách sử dụng các dịch vụ AWS như **ECS**, **CodeDeploy**, **ALB**, **CloudWatch**, **X-Ray**, **CodePipeline** để triển khai một chiến lược canary hoàn chỉnh.

- Thiết lập một quy trình **CI/CD** tự động, hỗ trợ **traffic shifting**, **giám sát**, **rollback tự động**, và **A/B testing**.

- Có khả năng **triển khai phiên bản mới an toàn**, giảm thiểu rủi ro và tối ưu trải nghiệm người dùng.

- Làm chủ công cụ **giám sát và phân tích hiệu suất sau triển khai**, từ đó cải thiện chất lượng release.

![AWS Architecture](/images/architecture.png)

### Mục tiêu

- Hiểu rõ khái niệm và lợi ích của Canary Deployment.

- Nắm kiến trúc triển khai thực tế trên AWS.

- Triển khai một pipeline Canary Deployment từ source code đến production ECS service.

- Thiết lập giám sát, cảnh báo, rollback và A/B testing cơ bản

- Tự động hóa toàn bộ quy trình CI/CD với rollback thông minh

### Yêu cầu

**Kiến thức nền tảng:**

- Kiến thức cơ bản về AWS (ECS, IAM, VPC, ALB).

- CI/CD và Git workflow

- Docker

**Tài nguyên cần chuẩn bị:**

- Tài khoản AWS .

- Repository code mẫu.

- Docker image đã có sẵn hoặc biết cách build.

### Nội dung

1. [Giới thiệu](1-introduction/)
2. [Kiến trúc triển khai](2-architecture/)
3. [Thiết lập môi trường](3-setup-environment/)
4. [Xây dựng CI/CD pipeline](4-build-cicd-pipeline/)
5. [Giám sát & tự động rollback](5-monitoring-rollback/)
6. [A/B Testing với ALB Listener](6-ab-testing-alb/)
7. [Demo thực tế](7-demo/)
