# 📂 HỒ SƠ CHIẾN LƯỢC: TỪ ZERO ĐẾN CLOUD SECURITY ARCHITECT

* **Chủ sở hữu:** Dương Tuấn Anh
* **Ngày bắt đầu:** 24/11/2025
* **Mục tiêu:** Thực tập (05/2026) -> Cloud Security Architect tại Big Tech.
* **Cam kết thời gian:** 15 - 20 giờ/tuần.

---

## 🚦 QUY ƯỚC TRẠNG THÁI (LEGEND)
- [ ] Bài chưa học (Not Started)
- [x] 🚧 **Bài đang học dở (In Progress)**
- [x] ✅ 🎉 **~~Bài đã hoàn thành (Done)~~**

---

## PHẦN 1: QUY TẮC TÁC CHIẾN (BẮT BUỘC)

1.  **Ưu tiên Sinh tồn (Academic First):** GPA & Môn đại cương (C++, Toán) là SỐ 1. Thi cử -> Dừng Cloud ngay lập tức.
2.  **Thủ công trước - Tự động sau (Manual First):** (1) Làm tay trên Console/Linux -> (2) Debug hiểu bản chất -> (3) Mới viết Code (Terraform/Script).
3.  **An toàn Thông tin (Security Hygiene):**
    * Luôn dùng `.gitignore`.
    * Kiểm tra AWS Billing sáng Thứ Hai ($10 Budget).
    * Lộ Key -> Xóa ngay.
4.  **Ký hiệu hành động:**
    * 🧠 **PHẢI HIỂU:** Lý thuyết cốt lõi (Bắt buộc đọc tài liệu để hiểu bản chất *tại sao*).
    * 🛠️ **CỨ LÀM THÔI:** Kỹ năng thực hành (Copy-paste, gõ cho quen tay, hiểu sau).

---

## PHẦN 2: CHIẾN THUẬT HỌC TẬP (LINH HOẠT)

*Bro tự đánh giá độ khó của bài Lab hôm nay để chọn cách tiếp cận:*

**TRƯỜNG HỢP A: Bài Nhỏ/Dễ (Vd: Lệnh Linux, Git cơ bản)**
* *Chiến thuật:* "Đánh nhanh thắng nhanh" (Gói gọn trong 1 tối).
* *Quy trình:* Đọc (15p) -> Làm Lab (30p) -> Viết Note/README -> Push Git -> **DONE.**

**TRƯỜNG HỢP B: Dự án Lớn/Khó (Vd: VPC, Web 3 Lớp, Terraform)**
* *Chiến thuật:* "Chia để trị" (Kéo dài 2-3 tối).
* *Tối 1 (Manual):* Đọc tài liệu + Làm thủ công trên Console -> Ghi lại lỗi.
* *Tối 2 (Debug/Auto):* Sửa lỗi + Viết code tự động hóa (Automation).
* *Tối 3 (Finalize):* Hoàn thiện README (Diagram + Threat Model) + Push Git.

**CUỐI TUẦN (Thứ 7 & CN):**
* **Thứ 7 (TỔNG KẾT):** Ôn lại kiến thức (Active Recall) + Viết LinkedIn + Dọn dẹp Resource AWS.
* **Chủ Nhật (NGHỈ NGƠI):** Cấm Code. Đi chơi, ngủ bù.

---

## PHẦN 3: NĂM NHẤT - SPRINT THỰC TẬP (11/2025 - 11/2026)

### 📍 Giai đoạn 1.1: Linux, Git & Tư duy Lập trình (24/11/2025 – 10/01/2026)

- [x] ✅ 🎉 **~~Setup Môi trường~~** 
    * 🛠️ *Cứ làm thôi:* Cài VS Code, Git, tạo Repo, copy file `.gitignore`. Bật AWS Billing Alarm ($10).
    > [!Note]
    > **Đã thao tác** Đã thao tác hết vào hôm 24 rồi nay mới update thêm vào đây
* [x] ✅ 🎉 **~~Git Mastery:~~**
    * 🛠️ *Cứ làm thôi:* Học thuộc `git init`, `add`, `commit`, `push`, `branch`.
    > [!Note]
    > Đã thực hành sơ qua `add`, `commit`, `push`.
    >
    > [!Note]
    >  Thực hành khá là nhiều với câu lệnh `add`, `commit` và `push` rồi
    * 🧠 *Phải hiểu:* Tại sao không được push file nhạy cảm (`.env`) lên Git?
    > [!Note]
    >  Có thể hiểu `.env`là két sắt thông tin của bản thân nếu public thì khác nào show hết bí mật mình muốn giấu lên mạng
* [x] ✅ 🎉 **~~Linux File System & Permissions:~~**
    * 🛠️ *Cứ làm thôi:* Gõ lệnh `ls`, `cd`, `mkdir`, `rm`, `chmod`, `chown`.
    > [!Note]
    >  Đã thực hành sơ qua ls, mkdir, cd, whoami.
    >
    > [!Note]
    >  Đã thực hành tạo file, xóa file, chmod 600 và chuyển quyền sở hữu cho root
    * 🧠 *Phải hiểu:* Cấu trúc thư mục `/etc`, `/var`. Tại sao `chmod 777` là nguy hiểm?
    > [!Note]
    >  Đã tìm hiểu và biết được nếu tạo lệnh `chmod 777` thì khác gì mình mở cửa nhà cho người ta vào muốn làm gì thì làm, muốn đập gì thì đập **777** này chỉ dùng để test thôi còn `chmod 600` là khóa quyền chỉ cho bản thân đọc, ghi, xóa thôi.
            Công thức: 7 = 4 (Đọc) + 2 (Ghi) + 1 (Chạy)
        3 con số 7 (7-7-7) nghĩa là:
        Chủ nhà (Bro): Full quyền.
        Nhóm bạn (Group): Full quyền.
        Người lạ (Everyone): FULL quyền.
    >
    > [!Note]
    >  Hơn hết Hacker (hoặc một user vớ vẩn nào đó) có thể chèn mã độc vào file của mình, hoặc xóa bay file đó mà không cần mật khẩu.
    >
    > [!Note]
    >  `/etc``(Editable Text Configuration-Cấu hình văn bản có thể chỉnh sửa)`: nó giống như `Control Panel` hoặc `Settings` ở Windows vậy nó chứa toàn bộ file cấu hình hệ thống ví dụ như: danh sách user, cấu hình mạng, cấu hình Web Server.... Nó khá là quan trọng bởi vì muốn đổi port web, muốn chặn IP... mình phải chui vào đây sửa file.
    >
    > [!Note]
    >  `/var` `(Variable - Biến đổi)`: có thể ví như `cuốn nhật ký` hoặc `Kho chứa đồ linh tinh` nó chứa những file thay đổi liên tục về kích thước. Quan trọng nhất là `Log Files (/var/log)`bởi vì nếu server bị lỗi hoặc bị hack, mình phải chui vào `/var/log` để đọc nhật ký xem chuyện gì đã xảy ra.
* [ ] **Linux Security Hardening:**
    * 🛠️ *Cứ làm thôi:* Copy lệnh tạo SSH Key (`ssh-keygen`), tắt Root Login.
    * 🧠 *Phải hiểu:* Public Key và Private Key khác nhau chỗ nào?
* [ ] **Automation Scripting:**
    * 🛠️ *Cứ làm thôi:* Copy mẫu script backup (`tar`, `cron`).
    * 🧠 *Phải hiểu:* Cronjob hoạt động ra sao?
* [ ] **MANDATORY LAB: Manual LAMP Stack** (Bài Lớn - Chia 2 tối):
    * 🛠️ *Cứ làm thôi:* Copy lệnh cài Apache, MySQL, PHP từng dòng một.
    * 🧠 *Phải hiểu:* File cấu hình Apache nằm ở đâu? Làm sao để start/stop service?
* [ ] **Project 0: CV tĩnh trên S3:**
    * 🛠️ *Cứ làm thôi:* Upload file HTML lên S3, bật Static Hosting.

### 📍 Giai đoạn 1.2: Mạng máy tính & Terraform Nhập môn (11/01 – 28/02)

* [ ] **Subnetting (Chia IP):**
    * 🧠 *Phải hiểu (SỐNG CÒN):* Nhìn vào `/24`, `/16` biết ngay có bao nhiêu IP. Phân biệt Public vs Private IP.
* [ ] **VLAN & ACL (Packet Tracer - Max 2 tuần):**
    * 🛠️ *Cứ làm thôi:* Cấu hình Switch/Router Cisco theo bài mẫu.
    * 🧠 *Phải hiểu:* Tại sao phải chia VLAN? Tại sao cần chặn traffic?
* [ ] **AWS VPC (Virtual Private Cloud - Bài Lớn):**
    * 🛠️ *Cứ làm thôi:* Bấm Console tạo VPC, Subnet, IGW.
    * 🧠 *Phải hiểu (SỐNG CÒN):* Luồng đi của gói tin. Tại sao Private Subnet cần NAT Gateway mới ra được Net?
* [ ] **Terraform Basic:**
    * 🛠️ *Cứ làm thôi:* Cú pháp HCL (`resource "aws_vpc"`). Copy docs là ra.
    * 🧠 *Phải hiểu:* **State File** là gì? Tại sao mất file này là mất toàn bộ hạ tầng?

### 📍 Giai đoạn 1.3: Dự án lớn & Nền tảng Ứng dụng (01/03 – 15/04)

* [ ] **Database & SQL:**
    * 🛠️ *Cứ làm thôi:* Gõ lệnh `SELECT`, `INSERT`, `UPDATE`, `JOIN`.
    * 🧠 *Phải hiểu:* Quan hệ 1-Nhiều là gì? Khóa chính (PK) vs Khóa ngoại (FK).
* [ ] **Mật mã học cơ bản (Cryptography):**
    * 🧠 *Phải hiểu:* Hashing khác Encryption chỗ nào? HTTPS bắt tay (Handshake) ra sao?
* [ ] **AWS Security (IAM & SG):**
    * 🛠️ *Cứ làm thôi:* Tạo User, Policy. Tạo Security Group mở port 80/22.
    * 🧠 *Phải hiểu:* Nguyên tắc Quyền tối thiểu. Stateful (SG) khác gì Stateless (NACL)?
* [ ] **Docker Basics:**
    * 🛠️ *Cứ làm thôi:* Copy mẫu `Dockerfile`, lệnh `docker build`, `docker run`.
    * 🧠 *Phải hiểu:* Docker Container khác gì Máy ảo (VM)?
* [ ] **PROJECT 1: 3-TIER ARCHITECTURE (Dự án Đinh - 2 Tuần):**
    * 🛠️ *Cứ làm thôi:* Deploy Web-App-DB thủ công. Viết code Terraform.
    * 🧠 *Phải hiểu:* Web gọi App qua port nào? App gọi DB qua port nào?
* [ ] **CI/CD Basic:**
    * 🛠️ *Cứ làm thôi:* Config GitHub Actions để build Docker.

### 📍 Giai đoạn 1.4: Đóng gói hồ sơ (16/04 – 30/05)

* [ ] **Threat Model (Tư duy bảo mật):**
    * 🧠 *Phải hiểu:* Nhìn vào sơ đồ Project 1, chỉ ra được điểm yếu bị hack.
* [ ] **Interview Prep:**
    * 🛠️ *Cứ làm thôi:* Học thuộc 5 câu chuyện STAR.

---

## PHẦN 4: LỘ TRÌNH NĂM 2 & 3 (TẦM NHÌN)

### Năm 2: Chuyên nghiệp & Tự động hóa
* [ ] **Chứng chỉ:** Thi đậu **AWS Solutions Architect Associate (SAA-C03)**.
* [ ] **Windows Server & AD:** Dựng Domain Controller, hiểu **Kerberos**, GPO.
* [ ] **Python for DevOps:** Học `boto3`, Lambda. Viết Bot tự động quét lỗi AWS.
* [ ] **Web Security (OWASP):** Hiểu SQL Injection, XSS. Dùng Burp Suite bắt gói tin.
* [ ] **Advanced Terraform:** Modules, State Locking (DynamoDB).
* [ ] **Kubernetes (K8s):** Kiến trúc Pod, Node, Cluster.

### Năm 3: Security Master & Big Tech
* [ ] **Chứng chỉ:** Thi đậu **AWS Certified Security – Specialty**.
* [ ] **Cloud Security Deep Dive:** **KMS Envelope Encryption**, WAF, Shield, Threat Modeling.
* [ ] **DevSecOps:** Tích hợp tool scan (SonarQube, Trivy) vào CI/CD.
* [ ] **Algorithm (Big Tech):** Luyện LeetCode (Blind 75).
* [ ] **System Design:** Thiết kế hệ thống lớn (CAP Theorem, Sharding).