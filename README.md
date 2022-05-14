# AWS Re/Start

![AWS Restart](/images/0001.png)

## 1. **Tài liệu**

#### 1.1.  Course Agenda

+ Các bạn xem **[Course Agenda](https://drive.google.com/drive/folders/1ZLkHO4c3jcinvn2AD4vl6z4XeH9PjIqj?usp=sharing)**

#### 1.2. Tài liệu

+ Các bạn xem **[Tài liệu](https://drive.google.com/drive/folders/1CPHvF4D8bbAnkVtLbhT3i1HPrKF3S-Ru?usp=sharing)**

## 2. **Tóm tắt kiến thức**

### 2.1. Nhóm dịch vụ **Compute**

<p align="center" width="100%">
    <img width="10%" src="./images/compute.png">
</p>

#### 2.1.1. Amazon Elastic Compute Cloud (Amazon EC2) 

<p align="center" width="100%">
    <img width="10%" src="./images/0002-ec2.png">
</p>


+ **Amazon EC2** giống với máy chủ ảo hoặc máy chủ vật lý truyền thống. EC2 có **khả năng khởi tạo nhanh , khả năng co dãn tài nguyên mạnh mẽ , linh hoạt**.
+ Máy chủ ảo : chia nhỏ máy chủ  vật lý thành **nhiều máy chủ ảo**, mục đích để **tận dụng tài nguyên tốt hơn**
+ **Amazon EC2** có thể hỗ trợ các workload như lưu trữ web, ứng dụng, cơ sở dữ liệu, dịch vụ xác thực và bất cứ công việc nào khác mà máy chủ thông thường có thể đáp ứng.

#### 2.1.2. Amazon EC2 Auto Scaling

<p align="center" width="100%">
    <img width="10%" src="./images/0003-ec2autoscaling.png">
</p>


+ **EC2 autoscaling :** Khả năng **tăng giảm** số máy chủ ảo , phụ thuộc vào lượng người dùng sử dụng ứng dụng

#### 2.1.3. AWS Lambda

<p align="center" width="100%">
    <img width="10%" src="./images/0004-awslambda.png">
</p>


+ **AWS Lambda :** dịch vụ tính toán **phi máy chủ** ( không có máy chủ ) xử lý công việc theo dạng các task nhỏ. 
+ Thực hiện xong công việc trả kết quả xong sẽ **tắt**.  
+ **Giảm** bớt công sức quản lý máy chủ ảo.

#### 2.1.4. AWS Elastic Beanstalk

<p align="center" width="100%">
    <img width="10%" src="./images/0005-awselasticbeanstalk.png">
</p>


+ **Elastic Beanstalk :** Dịch vụ giúp việc **quản lý** các tài nguyên AWS liên quan tới cùng 1 ứng dụng dễ dàng hơn.


### 2.2 Nhóm dịch vụ **Container**

<p align="center" width="100%">
    <img width="10%" src="./images/0006-awscontainer.png">
</p>


#### 2.2.1. Amazon Elastic Container Service (Amazon ECS)

<p align="center" width="100%">
    <img width="10%" src="./images/0007-awsecs.png">
</p>


+ **Amazon ECS** là dịch vụ **quản lý container** với khả năng **mở rộng cao** cho phép đơn giản hóa việc chạy, ngừng chạy và quản lý các container trong cluster. 
+ Container sẽ được định nghĩa trong các **task definition** nhằm chạy các task đơn lẻ hoặc nhiều task trong một service.

#### 2.2.2. Amazon Elastic Container Registry (Amazon ECR)

<p align="center" width="100%">
    <img width="10%" src="./images/0008-awsecr.png">
</p>


+ **AWS ECR** là một dịch vụ **Docker container registry** quản lý hoàn toàn bởi **AWS** nhằm đơn giản hóa việc **lưu trữ, quản lý và triển khai** các Docker container image.
+ ECR có thể **tích hợp** được với **Amazon Elastic Container Service (ECS)** nhằm đơn giản hóa việc thiết lập luồng thực hiện triển khai cho các hệ thống production cũng như loại bỏ đi sự phức tạp trong việc quản lý kho lưu trữ cho các container image.


#### 2.2.3. Amazon Elastic Kubernetes Service (Amazon EKS)

<p align="center" width="100%">
    <img width="10%" src="./images/0009-awseks.png">
</p>


+ **Amazon Elastic Kubernetes Service (Amazon EKS)** là một dịch vụ **container orchestration** được quản lý bởi **AWS** giúp chúng ta để **tạo, quản lý, khởi chạy và thay đổi quy mô** các ứng dụng **Kubernetes** trong môi trường AWS hoặc cả môi trường **on-premise**.

#### 2.2.4. AWS Fargate 

<p align="center" width="100%">
    <img width="10%" src="./images/00010-awsfargate.png">
</p>


+ **AWS Fargate** là một công cụ điện toán **phi máy chủ**, thanh toán theo mức sử dụng cho phép bạn tập trung vào việc xây dựng ứng dụng mà không cần quản lý máy chủ.
+ **AWS Fargate** tương thích với cả **Amazon Elastic Container Service(ECS)** và **Amazon Elastic Kubernetes Service (EKS)**.

### 2.3. Nhóm dịch vụ **Networking and Content Delivery**

<p align="center" width="100%">
    <img width="10%" src="./images/00011-networking.png">
</p>


#### 2.3.1. Amazon VPC

<p align="center" width="100%">
    <img width="10%" src="./images/00012-vpc.png">
</p>


+ **Amazon Virtual Private Cloud (Amazon VPC)** cho phép bạn khởi chạy các tài nguyên AWS vào **một mạng ảo** mà bạn đã xác định.
+ VPC nằm trong **1 Region** , khi tạo VPC cần khai báo 1 lớp mạng **CIDR IPv4** ( bắt buộc ) và IPv6 (tùy chọn )
+ Giới hạn của VPC hiện tại là **5 VPC trên 1 AWS Region** trên **1 AWS Account**.
+ Mục đích chính sử dụng VPC thường dùng để **phân tách các môi trường**.

#### 2.3.2. Elastic Load Balancing ( ELB )

<p align="center" width="100%">
    <img width="10%" src="./images/00013-elb.png">
</p>


+ **Elastic Load Balancing ( ELB )** là một dịch vụ **cân bằng tải** được quản lý bởi **AWS** , có chức năng **phân phối lưu lượng** cho nhiều EC2 Instance hoặc Container . 
+ Sử dụng giao thức **HTTP, HTTPS, TCP và SSL (TCP bảo mật)**.
+ Có thể nằm ở **public hoặc private subnet**.  
+ Mỗi ELB sẽ được cấp tên DNS và kết nối thông qua DNS. 
+ Chỉ có Network Load Balancer hỗ trợ gán IP tĩnh.

#### 2.3.3. Amazon CloudFront

<p align="center" width="100%">
    <img width="10%" src="./images/00014-cloudfront.png">
</p>


+ **Amazon CloudFront** là dịch vụ **phân phối nội dung toàn cầu (CDN)** giúp phân phối một cách bảo mật **dữ liệu, video, ứng dụng và các API** đến người xem với **độ trễ thấp và tốc độ truyền cao.**

#### 2.3.4. AWS Transit Gateway

<p align="center" width="100%">
    <img width="10%" src="./images/00015-transitgateway.png">
</p>


+ **Transit Gateway** được dùng để **kết nối các VPC và mạng on-premises** thông qua một hub trung tâm. Điều này đơn giản hóa mạng và kết thúc các mối quan hệ định tuyến phức tạp. 
+ Transit Gateway Attachment là một công cụ để gán các subnet của từng VPC cần kết nối với nhau vào một TGW đã được khởi tạo. Transit Gateway Attachment hoạt động ở quy  mô Availability Zone (AZ-level). 
+ Trong VPC, khi một subnet ở một AZ có Transit Gateway Attachment với một TGW, các subnet khác trong cùng AZ đều có thể kết nối tới TGW đó

#### 2.3.5. Amazon Route 53

<p align="center" width="100%">
    <img width="10%" src="./images/00016-route53.png">
</p>


+ Amazon Route 53 là một dịch vụ web đám mây (DNS) có khả năng **duy trì mở rộng cao**, **định tuyến end user** đến các ứng dụng Internet

#### 2.3.6 AWS Direct Connect

<p align="center" width="100%">
    <img width="10%" src="./images/00017-directconnect.png">
</p>


+ **AWS Direct Connect** là dịch vụ cho phép **tạo kết nối riêng** từ trung tâm dữ liệu truyền thống tới AWS
+ Độ trễ khoảng **20 ms – 30 ms**.  
+ AWS Direct Connect ở Việt Nam hiện tại sẽ thông qua AWS Direct Connect partners và hoạt động dưới dạng **Hosted Connections**. ( Nếu trực tiếp tới AWS thì là **Dedicated Connections** )  
+ Băng thông Direct Connect có thể thay đổi **lên / xuống tùy nhu cầu.**

#### 2.3.7. AWS VPN

<p align="center" width="100%">
    <img width="10%" src="./images/00018-vpn.png">
</p>


+  Muốn **kết nối giữa on-premise server và AWS** một cách bảo mật mà không cần nối qua Internet thì VPN là một giải pháp hiệu quả.
+ **VPN Site to Site** dùng trong mô hình hybrid để thiết lập kết nối liên tục giữa môi trường trung tâm dữ liệu truyền thống tới môi trường VPC của AWS. 
+ Việc thiết lập kết nối sẽ cần 2  đầu endpoint ở phía AWS và phía khách hàng :
  + **Virtual Private Gateway** : Được quản lý hoàn toàn bởi AWS ( chia 2 endpoints ở 2 đầu AZ ).
  + **Customer Gateway** : Đầu endpoint phía khách hàng, có thể là thiết bị phần cứng hoặc software appliance.

### 2.4. Nhóm dịch vụ **Storage**

<p align="center" width="100%">
    <img width="10%" src="./images/00019-storage.png">
</p>


#### 2.4.1. Amazon Simple Storage Service (S3)

<p align="center" width="100%">
    <img width="10%" src="./images/00020-s3.png">
</p>


+ **Amazon S3** là kho lưu trữ ở mức **đối tượng**, có nghĩa là nếu muốn thay đổi một phần của tập tin, bạn phải thực hiện thay đổi rồi tải lại toàn bộ tập tin đã sửa đổi.

+ S3 phù hợp với các loại dữ liệu ghi một lần đọc nhiều lần **( WORM – Write Once Read Many)**

#### 2.4.2. Amazon Elastic Block Store (EBS) 

<p align="center" width="100%">
    <img width="10%" src="./images/00021-ebs.png">
</p>


+ **Amazon EBS** cung cấp **block storage** và được gán trực tiếp vào EC2 Instance , tuy được gán trực tiếp như 1 RAW device, EBS về bản chất hoạt động độc lập với EC2 và được kết nối thông qua mạng riêng của EBS.
+ EBS có hai nhóm đĩa chính là **HDD và SSD**, được thiết kế để đạt **độ sẵn sàng 99.999%** bằng cách replicate dữ liệu giữa **3 Storage Node trong 1 AZ**

#### 2.4.3. Amazon Elastic File System (EFS)

<p align="center" width="100%">
    <img width="10%" src="./images/00022-efs.png">
</p>


+ **EFS ( Elastic File System )** cho phép tạo các **NFSv4 Network volume** và gán vào nhiều EC2 Instances cùng lúc, quy mô lưu trữ lên đến hàng petrabyte. 

+ EFS chỉ support **Linux**.  
+ Sử dụng EFS chỉ tính chi phí theo dung lượng sử dụng ( trong khi EBS tính phí theo dung lượng cấp phát ).

+ EFS có thể được cấu hình để **mount** vào môi trường **on-premise qua DX hoặc VPN**.

### 2.5. Nhóm dịch vụ **Database**

<p align="center" width="100%">
    <img width="10%" src="./images/00023-database.png">
</p>


#### 2.5.1. Amazon Relational Database Service (Amazon RDS)

<p align="center" width="100%">
    <img width="10%" src="./images/00024-rds.png">
</p>


+ Là **cơ sở dữ liệu** được quản lý trên AWS, chúng ta chỉ truy cập và quản lý ở mức RDBMS , không thể truy cập và quản lý ở mức hệ điều hành. 
+ Bao gồm **Aurora, MySQL, Postgre SQL , MSSQL, Oracle , Maria.**

#### 2.5.2. Amazon Aurora

<p align="center" width="100%">
    <img width="10%" src="./images/00025-aurora.png">
</p>


+ **Amazon Aurora** là một công cụ **cơ sở dữ liệu quan hệ** được tối ưu lại hạ tầng lưu trữ bên dưới , cho hiệu năng **đọc ghi song song** cao. 
+ Nền tảng RDBMS có 2 lựa chọn là **MySQL và PostgreSQL**.

#### 2.5.3. Amazon RedShift

<p align="center" width="100%">
    <img width="10%" src="./images/00026-redshift.png">
</p>


+ **Amazon Redshift** là dịch vụ **Data warehouse** được quản lý bởi AWS. 
+ Lõi là **Postgresql** nhưng được tối ưu cho **OLAP**.

#### 2.5.4. Amazon Dynamo

<p align="center" width="100%">
    <img width="10%" src="./images/00027-dynamodb.png">
</p>


+ **Amazon Dynamodb** là dịch vụ **CSDL NoSQL** dạng **Key-Value , Key-Document** nhanh và linh hoạt được quản lý bởi AWS.

### 2.6. Nhóm dịch vụ **AWS Cost Management**

<p align="center" width="100%">
    <img width="10%" src="./images/00028-costmanagement.png">
</p>


#### 2.6.1. AWS Cost and Usage Report

<p align="center" width="100%">
    <img width="10%" src="./images/00029-costusagereport.png">
</p>


+ **AWS Cost & Usage Report** chứa những thông tin cụ thể nhất về **dữ liệu chi phí và mức sử dụng**. 
+ Nó bao gồm những siêu dữ liệu được bổ sung về ***dịch vụ AWS, giá cả và các phương án trả trước** ( ví dụ: Amazon EC2 Reserved Instances)

#### 2.6.2. AWS Budgets

<p align="center" width="100%">
    <img width="10%" src="./images/00030-awsbudget.png">
</p>


+ **AWS Budget** là một dịch vụ cung cấp khả năng **thiết lập ngân sách** để gửi cảnh báo cho bạn khi chi phí vượt quá chi phí mà ngân sách cho phép (hoặc được dự báo sẽ vượt quá ngân sách).

#### 2.6.3. AWS Cost Explorer

<p align="center" width="100%">
    <img width="10%" src="./images/00031-awscostexplorer.png">
</p>


+ **AWS Cost Explorer** cung cấp báo cáo mặc định giúp bạn **theo dõi chi phí và mức sử dụng** liên quan đến năm dịch vụ AWS tích lũy chi phí hàng đầu
+ Cung cấp cho bạn **bảng phân tích chi tiết** về tất cả dịch vụ ở chế độ xem bảng.


### 2.7. Nhóm dịch vụ **Security**

<p align="center" width="100%">
    <img width="10%" src="./images/00032-security.png">
</p>


#### 2.7.1.  Identity and Access Management (IAM) 

<p align="center" width="100%">
    <img width="10%" src="./images/00033-iam.png">
</p>


+ **IAM** là dịch vụ giúp bạn **kiểm soát quyền truy cập** vào các dịch vụ và tài nguyên trong AWS account của mình. 
+ IAM cho phép bạn **tạo nhiều tài khoản** người dùng ( IAM user ) với **thông tin xác thực** ( credentials ) và **quyền hạn** khác nhau.

#### 2.7.2. AWS Organizations

<p align="center" width="100%">
    <img width="10%" src="./images/00034-awsorganizations.png">
</p>


+ **AWS Organizations** giúp **quản lý và điều hành tập trung** môi trường của mình bao gồm nhiều AWS account.
+ AWS Organizations có thể **tạo các tài khoản AWS mới và phân bổ tài nguyên**, sắp xếp các AWS account theo **OU ( Organization Unit )**, đồng thời đơn giản việc **thanh toán tập trung**.

#### 2.7.3. Amazon Cognito

<p align="center" width="100%">
    <img width="10%" src="./images/00035-cognito.png">
</p>


+ **Amazon Cognito** là dịch vụ được quản lý bởi AWS có chức năng **xác thực, cấp phép và quản lý người dùng** cho các ứng dụng web và di động. 
+ Người dùng có thể **đăng nhập** trực tiếp bằng tên người dùng và mật khẩu hoặc thông qua một bên thứ ba như **Facebook, Amazon hoặc Google**.

#### 2.7.4. AWS Artifact

<p align="center" width="100%">
    <img width="10%" src="./images/00036-artifact.png">
</p>


+ **AWS Artifact** là **tài nguyên tập trung, tổng hợp** cho thông tin liên quan đến việc tuân thủ quan trọng đối với bạn. 
+ Tài nguyên này cung cấp **quyền truy cập** theo nhu cầu vào các **báo cáo bảo mật** và tuân thủ của AWS cũng như một số thỏa thuận trực tuyến.

#### 2.7.5. AWS Key Management Service (AWS KMS)

<p align="center" width="100%">
    <img width="10%" src="./images/00037-kms.png">
</p>


+ **AWS Key Management Service** giúp tạo và quản lý các **encryption key**, phục vụ cho mục đích **encrypt/decrypt** dữ liệu trên AWS . ( Encryption at rest )  
+ Encryption key luôn nằm trong AWS KMS , đảm bảo tiêu chuẩn FIPS 140-2.  
+ CMK ( Customer Managed Key ) đóng vai trò là tài nguyên chính trong AWS KMS. 
+ CMK có thể có kích thước tới 4KB. 
+ Tuy nhiên thông thường, chúng ta chỉ sử dụng CMK cho mục đích tạo, mã hóa và giải mã Data Key – loại khóa được dùng bên ngoài AWS KMS để mã hóa dữ liệu.

#### 2.7.6. AWS Shield 

<p align="center" width="100%">
    <img width="10%" src="./images/00038-shield.png">
</p>


+ **AWS Shield** là dịch vụ bảo vệ khỏi tấn công **Từ chối dịch vụ phân tán (DDoS)** gúp bảo vệ các ứng dụng chạy trên AWS.

### 2.8. Nhóm dịch vụ **Management and Governance**

<p align="center" width="100%">
    <img width="10%" src="./images/00039-managementandgovernance.png">
</p>


#### 2.8.1. AWS Management Console

<p align="center" width="100%">
    <img width="10%" src="./images/00040-awsmanagementconsole.png">
</p>


+ **AWS Management Console** là một ứng dụng web/di động dùng để **quản lý điều khiển các dịch vụ** của Amazon Web Services. 
+ Khi bạn đăng nhập lần đầu tiên, bạn sẽ thấy trang chủ của trình quản lý dịch vụ AWS. 
+ Trình quản lý điều khiển dịch vụ AWS sẽ bao gồm danh sách các dịch vụ khác nhau để lựa chọn sử dụng.

#### 2.8.2. AWS Config

<p align="center" width="100%">
    <img width="10%" src="./images/00041-awsconfig.png">
</p>


+ **AWS Config** là dịch vụ cho phép bạn **ước lượng, kiểm tra và đánh giá cấu hình** các tài nguyên AWS của bạn. 
+ **Config** sẽ liên tục theo dõi và ghi hồ sơ các cấu hình tài nguyên AWS của bạn và cho phép bạn tự động hóa việc đánh giá các cấu hình được ghi lại so với các cấu hình mong muốn.

#### 2.8.3. AWS CloudWatch

<p align="center" width="100%">
    <img width="10%" src="./images/00041-awscloudwatch.png">
</p>


+ **Amazon CloudWatch** là một công cụ cho phép bạn **thu thập dữ liệu** về hoạt động của các tài nguyên, ứng dụng, và dịch vụ đang vận hành trên AWS Cloud hoặc máy chủ của bạn. 
+ Dữ liệu thu thập được sẽ được lưu dưới dạng các **nhật ký, chỉ số, và sự kiện**. 
+ Cloudwatch cũng có thể thể hiện dữ liệu dưới **dạng biểu đồ** để bạn dễ dàng hình dung và chắt lọc thông tin từ dữ liệu.

#### 2.8.4. AWS Auto Scaling

<p align="center" width="100%">
    <img width="10%" src="./images/00042-awsautoscaling.png">
</p>


+ **AWS Auto Scaling** là tính năng **tự động nhân rộng** để đảm bảo rằng các phiên bản Amazon EC2 đủ để chạy các ứng dụng của bạn. 
+ Bạn có thể tạo một nhóm AWS Auto Scaling trong các phiên bản EC2.

#### 2.8.5. AWS Command Line Interface

<p align="center" width="100%">
    <img width="10%" src="./images/00043-cli.png">
</p>


+ **AWS Command Line Interface (AWS CLI)** là một công cụ **mã nguồn mở** (open source)
+ Dùng **tương tác với các dịch vụ AWS** bằng cách sử dụng các lệnh trong **cửa sổ lệnh** (command-line shell). 

#### 2.8.6. AWS Trusted Advisor

<p align="center" width="100%">
    <img width="10%" src="./images/00044-trustedadvisor.png">
</p>


+ **AWS Trusted Advisor** cung cấp các **đề xuất** giúp bạn tuân theo những **biện pháp thực hành tốt nhất** về AWS. 
+ Trusted Advisor đánh giá tài khoản của bạn bằng các nội dung kiểm tra.


#### 2.8.7. AWS Well-Architected Tool

<p align="center" width="100%">
    <img width="10%" src="./images/00045-Well-ArchitectedTool.png">
</p>


+ **AWS Well-Architected Tool** có sẵn miễn phí trong Bảng điều khiển quản lý AWS, cung cấp **cơ chế** để thường xuyên **đánh giá khối lượng công việc, xác định các vấn đề rủi ro** cao và **ghi lại các cải tiến**.

#### 2.8.8. CloudTrail

<p align="center" width="100%">
    <img width="10%" src="./images/00046-CloudTrail.png">
</p>


+ **CloudTrail** là dịch vụ **ghi lại các lệnh gọi API (API call )** AWS cho tài khoản của bạn và **lưu thông tin vào log.** 
+ Tương tác tới tài khoản AWS của bạn thông qua **Managment Console , CLI hay SDK** đều là các lệnh gọi API.


### 3. **Câu hỏi FAQ**


### Các bạn đặt câu hỏi tại [AWS Re/Start FAQ](https://docs.google.com/document/d/1bLPB57WPRGkpvGAAUpuV5cWn3DVQJrhpVL7LOWkMHJg/edit?usp=sharing)


#### 3.1 Amazon Elastic Compute Cloud (Amazon EC2) 

+ Xem các câu hỏi thường gặp về [Amazon Elastic Compute Cloud (Amazon EC2)](https://aws.amazon.com/vi/ec2/faqs/) 

#### 3.2. Amazon EC2 Auto Scaling

+ Xem các câu hỏi thường gặp về [Amazon EC2 Auto Scaling](https://aws.amazon.com/vi/ec2/autoscaling/faqs/)

#### 3.3. AWS Lambda

+ Xem các câu hỏi thường gặp về [AWS Lambda](https://aws.amazon.com/vi/lambda/faqs/)

#### 3.4. AWS Elastic Beanstalk

+ Xem các câu hỏi thường gặp về [AWS Elastic Beanstalk](https://aws.amazon.com/vi/elasticbeanstalk/faqs/)

#### 3.5. Amazon ECS

+ Xem các câu hỏi thường gặp về [Amazon ECS](https://aws.amazon.com/vi/ecs/faqs/)

#### 3.6. Amazon ECR

+ Xem các câu hỏi thường gặp về [Amazon ECR](https://aws.amazon.com/vi/ecr/faqs/)

#### 3.7. Amazon EKS

+ Xem các câu hỏi thường gặp về [Amazon EKS](https://aws.amazon.com/vi/eks/faqs/)

#### 3.8. AWS Fargate

+ Xem các câu hỏi thường gặp về [AWS Fargate](https://www.amazonaws.cn/en/fargate/faqs/)

#### 3.9. Amazon VPC

+ Xem các câu hỏi thường gặp về [Amazon VPC](https://aws.amazon.com/vi/vpc/faqs/)

#### 3.10. Elastic Load Balancing

+ Xem câu hỏi thường gặp về [Elastic Load Balancing](https://aws.amazon.com/vi/elasticloadbalancing/faqs/)

#### 3.11. Amazon CloudFront

+ Xem các câu hỏi thường gặp về [Amazon CloudFront](https://aws.amazon.com/vi/cloudfront/faqs/)

#### 3.12. AWS Transit Gateway

+ Xem các câu hỏi thường gặp về [AWS Transit Gateway](https://aws.amazon.com/vi/transit-gateway/faqs/)

#### 3.13. Amazon Route 53

+ Xem các câu hỏi thường gặp về [Amazon Route 53](https://aws.amazon.com/vi/route53/faqs/)

#### 3.14. AWS Direct Connect

+ Xem các câu hỏi thường gặp về [AWS Direct Connect](https://aws.amazon.com/vi/directconnect/faqs/)

#### 3.15. AWS VPN 

+ Xem các câu hỏi thường gặp về [AWS VPN](https://aws.amazon.com/vi/vpn/faqs/)

#### 3.16. AWS S3

+ Xem các câu hỏi thường về [AWS S3](https://aws.amazon.com/vi/s3/faqs/)

#### 3.17. Amazon EBS

+ Xem các câu hỏi thường gặp về [Amazon EBS](https://aws.amazon.com/vi/ebs/faqs/)

#### 3.18. Amazon EFS

+ Xem các câu hỏi thường gặp về [Amazon EFS](https://aws.amazon.com/vi/ebs/faqs/)

#### 3.19. AWS RDS

+ Xem các câu hỏi thường gặp về [AWS RDS](https://aws.amazon.com/vi/rds/faqs/)

#### 3.20. Amazon Aurora

+ Xem các câu hỏi thường gặp về [Amazon Aurora](https://aws.amazon.com/vi/rds/aurora/faqs/)

#### 3.21. Amazon RedShift

+ Xem các câu hỏi thường gặp về [Amazon RedShift](https://aws.amazon.com/vi/redshift/faqs/)

#### 3.22. Amazon Dynamo

+ Xem các câu hỏi thường gặp về [Amazon Dynamo](https://aws.amazon.com/vi/dynamodb/faqs/)

#### 3.23. AWS Cost and Usage Report

+ Xem các câu hỏi thường gặp về [AWS Cost and Usage Report](https://aws.amazon.com/vi/aws-cost-management/aws-cost-and-usage-reporting/faqs/)

#### 3.24. AWS Budgets

+ Xem các câu hỏi thường gặp về [AWS Budgets](https://aws.amazon.com/vi/aws-cost-management/aws-budgets/faqs/)

#### 3.25. AWS Cost Explorer

+ Xem các câu hỏi thường gặp về [AWS Cost Explorer](https://aws.amazon.com/vi/aws-cost-management/faqs/)

#### 3.26. IAM

+ Xem các câu hỏi thường gặp về [IAM](https://aws.amazon.com/vi/iam/faqs/)

#### 3.27. AWS Organizations

+ Xem các câu hỏi thường gặp về [AWS Organizations](https://aws.amazon.com/vi/organizations/faqs/) 

#### 3.28. Amazon Cognito

+ Xem các câu hỏi thường gặp về [Amazon Cognito](https://aws.amazon.com/vi/cognito/faqs/)   

#### 3.29. AWS Artifact

+ Xem các câu hỏi thường gặp về [AWS Artifact](https://aws.amazon.com/vi/artifact/faq/)    

#### 3.30. AWS KMS

+ Xem các câu hỏi thường gặp về [AWS KMS](https://aws.amazon.com/vi/kms/faqs/)   

#### 3.31. AWS Shield

+ Xem các câu hỏi thường gặp về [AWS Shield](https://aws.amazon.com/vi/shield/faqs/)   

#### 3.32. AWS Management Console

+ Xem các câu hỏi thường gặp về [AWS Management Console](https://aws.amazon.com/vi/console/faq-console/)    

#### 3.33. AWS Config

+ Xem các câu hỏi thường gặp về [AWS Config ](https://aws.amazon.com/vi/config/faq/)     

#### 3.34. AWS CloudWatch

+ Xem các câu hỏi thường gặp về [AWS CloudWatch](https://aws.amazon.com/vi/cloudwatch/faqs/)    

#### 3.35. AWS Auto Scaling

+ Xem các câu hỏi thường gặp về [AWS Auto Scaling](https://aws.amazon.com/vi/autoscaling/faqs/)   

#### 3.36. AWS CLI

+ Xem các câu hỏi thường gặp về [AWS CLI](https://aws.amazon.com/vi/cli/)    

#### 3.37. AWS Trusted Advisor

+ Xem các câu hỏi thường gặp về [AWS Trusted Advisor](https://www.amazonaws.cn/en/support/trustedadvisor/faq/)    

#### 3.38. AWS Well-Architected Tool

+ Xem các câu hỏi thường gặp về [AWS Well-Architected Tool](https://aws.amazon.com/vi/well-architected-tool/faqs/)   

#### 3.39. AWS CloudTrail

+ Xem các câu hỏi thường gặp về [ AWS CloudTrail](https://aws.amazon.com/vi/cloudtrail/faqs/)   


### 4. **[Extra mission](https://van-hoang-kha.github.io/FCJ-Special-Force/)**


