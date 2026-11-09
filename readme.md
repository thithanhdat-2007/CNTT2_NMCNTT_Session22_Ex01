# BÀI TẬP 1: SỬ DỤNG PHỐI HỢP CÁC TOÁN TỬ TÌM KIẾM NÂNG CAO ĐỂ TÌM TÀI LIỆU CHÍNH THỐNG

## I. Đề bài & Yêu cầu

1. **Mục tiêu**: Sử dụng phối hợp các toán tử tìm kiếm nâng cao để tìm kiếm tài liệu chính thống, tránh mã độc.
2. **Bối cảnh (Roleplay)**: Bạn là sinh viên đang cần tìm cuốn giáo trình "Nhập môn Công nghệ Thông tin" bản PDF của Học viện để ôn thi, nhưng kết quả Google toàn trả về các trang web bắt nạp thẻ hoặc quảng cáo bài viết không liên quan.
3. **Yêu cầu nghiệp vụ**:
   - Viết một chuỗi truy vấn (Query) sử dụng toán tử `filetype:`, `site:` và dấu ngoặc kép `" "` để tìm trực tiếp tệp tin PDF trên máy chủ của trường (`ptit.edu.vn`).
   - Sử dụng toán tử trừ `-` để loại bỏ ít nhất 2 trang web "rác" thường xuyên xuất hiện trong kết quả tìm kiếm.
4. **Yêu cầu đầu ra**:
   - Mô tả tại sao việc dùng toán tử `filetype:` lại giúp tiết kiệm thời gian hơn so với việc gõ "tải sách..." thông thường.
   - Ảnh chụp màn hình và 3 kết quả đầu tiên sau khi áp dụng "Combo toán tử".

## II. Bài làm chi tiết

### Câu 1: Chuỗi truy vấn tìm kiếm nâng cao (Combo toán tử)

**Chuỗi truy vấn áp dụng cho Học viện Công nghệ Bưu chính Viễn thông (`ptit.edu.vn`):**

```text
"Nhập môn Công nghệ Thông tin" filetype:pdf site:ptit.edu.vn -site:123docz.net -site:tailieu.vn
```

*(Hoặc chuỗi truy vấn mở rộng cho toàn bộ khối các trường Đại học/Học viện tại Việt Nam)*:

```text
"Nhập môn Công nghệ Thông tin" filetype:pdf site:edu.vn -site:123docz.net -site:tailieu.vn -site:scribd.com
```

**Phân tích vai trò của từng toán tử trong câu lệnh:**
* **Dấu ngoặc kép `"Nhập môn Công nghệ Thông tin"`**: Bắt buộc công cụ tìm kiếm chỉ trả về các tài liệu chứa chính xác cụm từ khóa này theo đúng thứ tự, không tách rời từng chữ đơn lẻ.
* **Toán tử `filetype:pdf`**: Chỉ lọc các liên kết trỏ trực tiếp tới tệp văn bản định dạng `.pdf`, loại bỏ hoàn toàn các trang bài viết `.html` thông thường.
* **Toán tử `site:ptit.edu.vn` (hoặc `site:edu.vn`)**: Giới hạn phạm vi tìm kiếm nằm gọn trong máy chủ chính thống của Học viện Công nghệ Bưu chính Viễn thông (bao gồm cả các tên miền phụ như `daotao.ptit.edu.vn`, `clc.ptit.edu.vn`).
* **Toán tử trừ `-site:123docz.net -site:tailieu.vn`**: Loại trừ triệt để các trang web lưu trữ trung gian thường xuyên chèn quảng cáo hoặc yêu cầu nạp tiền/nạp thẻ VIP mới cho phép tải tài liệu.

### Câu 2: Tại sao dùng toán tử `filetype:` giúp tiết kiệm thời gian và tránh mã độc hơn cách gõ "tải sách..." thông thường?

* **Trỏ trực tiếp đến tệp tin gốc trên máy chủ**: Khi gõ cụm từ thông thường như `"tải sách Nhập môn Công nghệ Thông tin"`, thuật toán tìm kiếm sẽ ưu tiên các trang web thương mại, blog hoặc diễn đàn tối ưu hóa từ khóa SEO "tải sách". Ngược lại, `filetype:pdf` ép Google chỉ hiển thị đường dẫn trực tiếp đến tệp PDF — nhấp chuột là mở đọc hoặc tải về ngay lập tức mà không cần đi qua trang trung gian.
* **Loại bỏ bẫy nạp thẻ và liên kết rút gọn quảng cáo**: Các trang web rác thường giăng bẫy từ khóa "tải sách miễn phí" để dẫn dụ sinh viên đọc thử vài trang đầu rồi bắt đăng ký tài khoản, nạp thẻ cào hoặc nhấp qua nhiều lớp link rút gọn chứa quảng cáo độc hại.
* **Ngăn chặn rủi ro tải nhầm mã độc (Malware/Adware)**: Nhiều trang web không chính thống gắn nút "Download/Tải xuống" giả mạo nhằm phát tán tệp thực thi chứa virus (`.exe`, `.apk`, `.msi`, `.zip`). Việc kết hợp `filetype:pdf` và `site:ptit.edu.vn` đảm bảo 100% tệp tải về là tài liệu học tập chuẩn từ máy chủ nhà trường.

### Câu 3: Ba kết quả đầu tiên sau khi áp dụng "Combo toán tử"

**1. Kết quả thực tế trên máy chủ Học viện Công nghệ Bưu chính Viễn thông (`site:ptit.edu.vn`):**
* **Kết quả 1**: [Chương trình đào tạo đại học ngành Công nghệ thông tin - PTIT (979qd_Chuong-trinh-dao-tao.pdf)](https://daotao.ptit.edu.vn/wp-content/uploads/sites/3/2024/08/979qd_Chuong-trinh-dao-tao.pdf) — Lưu trữ trên cổng Đào tạo của Học viện (`daotao.ptit.edu.vn`).
* **Kết quả 2**: [Chương trình khung đào tạo ngành CNTT - Học viện Công nghệ Bưu chính Viễn thông](https://ptit.edu.vn/giaovu/wp-content/uploads/2020/12/CHUONG-TRINH-KHUNG-DAO-TAO-KHOA-2019-NGANH-CNTT-1.pdf) — Lưu trữ trên chuyên trang Giáo vụ của Học viện (`ptit.edu.vn/giaovu`).
* **Kết quả 3**: [Phụ lục ĐH18 - Chương trình đào tạo Cử nhân Công nghệ thông tin (định hướng ứng dụng) - PTIT](https://ptit.edu.vn/wp-content/uploads/2024/10/1.-Bieu-mau-17-Phu-luc-DH18.CNTT-UDU.pdf) — Lưu trữ trực tiếp trên máy chủ chính của Học viện (`ptit.edu.vn`).

**2. Kết quả thực tế khi mở rộng trên toàn khối trường Đại học/Học viện (`site:edu.vn`):**
* **Kết quả 1**: [NHẬP MÔN CÔNG NGHỆ THÔNG TIN VÀ TRUYỀN THÔNG - SoICT](https://users.soict.hust.edu.vn/huonglt/IT/Bai%201-Gioi-thieu-Vien-CNTTTT-va-CTDT.pdf) — Bài giảng lưu trữ trên máy chủ Trường CNTT&TT – ĐH Bách khoa Hà Nội (`soict.hust.edu.vn`).
* **Kết quả 2**: [Chương trình đào tạo Ngành Công nghệ thông tin - Trường Đại học Gia Định](https://giadinh.edu.vn/e-img/files/CHUONG%20TRINH%20DAO%20TAO%20UP%20WEB.pdf) — Tài liệu đề cương môn Nhập môn CNTT trên máy chủ `giadinh.edu.vn`.
* **Kết quả 3**: [Chương trình đào tạo Công nghệ thông tin - HCMUS](https://hcmus.edu.vn/wp-content/uploads/2024/03/CTDT-K-2020_Cong-nghe-thong-tin.pdf) — Tài liệu lưu trữ trên máy chủ Trường ĐH Khoa học Tự nhiên – ĐHQG-HCM (`hcmus.edu.vn`).
