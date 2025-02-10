---
title : "Dọn dẹp tài nguyên"
date :  "2025-02-08" 
weight : 6 
chapter : false
pre : " <b> 6. </b> "
---

{{% notice info %}}
Sau khi dự án đã được triển khai và hoạt động ổn định, việc dọn dẹp và quản lý các tài nguyên đã sử dụng trong quá trình phát triển là rất quan trọng. Điều này không chỉ giúp bạn tránh được các chi phí không cần thiết mà còn duy trì một môi trường làm việc hiệu quả. Dưới đây là các bước để tối ưu và dọn dẹp tài nguyên AWS đã tạo ra trong suốt dự án
{{% /notice %}}

#### 1. Xóa các Instances AWS EC2
Việc xóa các EC2 instances AWS là cần thiết để quản lý chi phí, vì nó giảm bớt các khoản phí không cần thiết cho các tài nguyên không sử dụng. Điều này cũng nâng cao bảo mật bằng cách giảm thiểu bề mặt tấn công, tối ưu hóa phân bổ tài nguyên, và cải thiện sự rõ ràng và tổ chức trong môi trường của bạn. Hơn nữa, việc xóa các instances lỗi thời định kỳ giúp đảm bảo tuân thủ các chính sách của tổ chức, làm cho đây trở thành một thực tiễn tốt nhất trong quản lý tài nguyên hiệu quả.

#### 2. Kiểm tra Dọn Dẹp
Sau khi xóa tài nguyên, điều quan trọng là kiểm tra xem tất cả các chi phí liên quan đã được loại bỏ hay chưa như một thực tiễn tốt. Bạn có thể sử dụng AWS Cost Explorer để theo dõi và xác nhận rằng không có khoản phí nào được tính từ các tài nguyên còn lại.

{{% notice note %}}
Bằng cách làm theo các bước này, bạn sẽ đảm bảo rằng môi trường AWS của mình đã được dọn dẹp đúng cách, giúp ngăn ngừa chi phí không cần thiết và duy trì một cơ sở hạ tầng đám mây gọn gàng, hiệu quả.
{{% /notice %}}