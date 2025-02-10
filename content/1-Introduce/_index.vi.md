---
title : "Giới thiệu"
date :  "2025-02-08" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

Trong ngành công nghiệp điện toán đám mây đang phát triển ngày nay, kiến trúc serverless đang thu hút sự chú ý đáng kể nhờ khả năng mở rộng, tiết kiệm chi phí và dễ dàng bảo trì. Dự án này của tôi sẽ trình bày cách xây dựng một chức năng đơn giản (đăng ký, đăng nhập) với Backend viết bằng Node.js, Frontend viết bằng Next.js, sử dụng cơ sở dữ liệu MongoDB và triển khai trên AWS bằng EC2. Công nghệ này cung cấp các công cụ mạnh mẽ để phát triển ứng dụng web có khả năng mở rộng và tiết kiệm chi phí với chi phí vận hành tối thiểu.

#### Tại sao sử dụng Node.js?
Node.js là một nền tảng phát triển ứng dụng web hiệu suất cao, cho phép xử lý nhiều kết nối đồng thời nhờ mô hình bất đồng bộ. Việc sử dụng JavaScript cho cả client và server giúp Node.js có một hệ sinh thái thư viện phong phú thông qua npm, dễ dàng mở rộng cho kiến trúc microservices và phù hợp với các ứng dụng thời gian thực. Cộng đồng lớn và cú pháp dễ học cũng là những điểm nổi bật của Node.js.

#### Tại sao sử dụng Next.js?
Next.js là một framework mạnh mẽ dành cho phát triển ứng dụng web, nổi bật với khả năng tối ưu hóa SEO nhờ Server-Side Rendering (SSR) và Static Site Generation (SSG). Nó cung cấp hiệu suất cao nhờ kỹ thuật chia nhỏ code và tải trang nhanh chóng. Next.js cũng dễ sử dụng với cấu trúc thư mục rõ ràng và hệ thống định tuyến tự động, giúp lập trình viên quản lý ứng dụng dễ dàng hơn.  
Ngoài ra, framework này cho phép xây dựng API trong cùng một dự án, tạo sự liền mạch giữa frontend và backend. Với các tính năng phong phú như tối ưu hóa hình ảnh, CSS Modules và hỗ trợ TypeScript, Next.js rất phù hợp cho các dự án hiện đại. Cộng đồng phát triển lớn và tài liệu phong phú cũng là điểm cộng giúp người dùng dễ dàng tìm kiếm sự hỗ trợ và thông tin.

#### Tại sao sử dụng MongoDB?
MongoDB là một cơ sở dữ liệu NoSQL linh hoạt, cho phép lưu trữ dữ liệu dưới dạng tài liệu, dễ dàng thay đổi cấu trúc mà không cần chỉnh sửa schema. Nó hỗ trợ phân tán dữ liệu và mở rộng theo chiều ngang, giúp xử lý lượng dữ liệu lớn với tốc độ truy vấn nhanh. MongoDB cũng dễ dàng tích hợp với nhiều ngôn ngữ lập trình, cung cấp khả năng truy vấn mạnh mẽ và có cộng đồng hỗ trợ lớn, trở thành một lựa chọn lý tưởng cho các ứng dụng hiện đại.

#### Tại sao sử dụng AWS EC2?
AWS EC2 (Elastic Compute Cloud) là một dịch vụ điện toán đám mây cho phép mở rộng linh hoạt, triển khai và quản lý máy chủ ảo dễ dàng chỉ trong vài phút. Nó cung cấp độ sẵn sàng cao với nhiều vùng và khu vực khác nhau, bảo mật mạnh mẽ và tích hợp dễ dàng với các dịch vụ AWS khác. Mô hình thanh toán theo nhu cầu giúp tối ưu hóa chi phí, khiến EC2 trở thành lựa chọn lý tưởng để triển khai ứng dụng hiện đại.

#### Workshop bao gồm 6 phần chính:
 1. [Giới thiệu](1-introduce/)
 2. [Chuẩn bị](2-preparation/)
    1. [Tải Visual Studio Code](2-preparation/2.1-vscode/)
    2. [Tạo AWS EC2 và kết nối instance](2-preparation/2.2-ec2/)
 3. [Triển khai Backend trên AWS EC2](3-deploybackend/)
 4. [Triển khai Frontend trên AWS EC2](4-deployfrontend/)
 5. [Kiểm tra và đánh giá ứng dụng](5-testing/)
 6. [Dọn dẹp tài nguyên](6-cleanup/)