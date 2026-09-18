# Smart Schedule - Thời Khóa Biểu Thông Minh (THCS Võ Cường)

Dự án website Thời Khóa Biểu thông minh được tái tạo và cấu trúc chuẩn hóa từ `code.txt`.

---

## 📁 Cấu trúc thư mục dự án

```text
Smart Schedule/
├── index.html            # Trang chính của ứng dụng (giao diện modular, sạch sẽ)
├── bundle.html           # Phiên bản đóng gói tất cả trong 1 file (dễ chia sẻ, chạy offline)
├── code.txt              # Mã nguồn gốc ban đầu
├── README.md             # Hướng dẫn sử dụng & cấu trúc dự án
├── css/
│   └── style.css         # Toàn bộ hiệu ứng CSS, in ấn A4, animation chữ 3D, thanh cuộn
└── js/
    ├── logger.js         # Ghi nhật ký lỗi và sự kiện ứng dụng
    ├── data.js           # Dữ liệu mẫu (môn học, khung giờ, hồ sơ học sinh, TKB mẫu)
    ├── firebase-config.js# Cấu hình đồng bộ dữ liệu đám mây qua Firebase Firestore
    ├── subjects.js       # Quản lý môn học (thêm, sửa, xóa, gắn màu)
    ├── storage.js        # Quản lý lưu trữ localStorage (đa hồ sơ, TKB, bài tập)
    ├── timetable.js      # Lưới thời khóa biểu tự động tính pixel theo khung giờ
    ├── homework.js       # Quản lý bài tập về nhà, hạn nộp, hiệu ứng pháo hoa
    ├── ocr-handler.js    # Nhận diện thời khóa biểu từ ảnh bằng AI (Tesseract OCR)
    └── app.js            # Điều phối toàn bộ ứng dụng (tabs, đồng hồ, hôm nay, admin, export)
```

---

## 🚀 Cách mở và sử dụng

1. **Mở trực tiếp (Không cần cài đặt thêm phần mềm)**:
   * Nhấp đúp vào tệp **`index.html`** để mở trên bất kỳ trình duyệt nào (Edge, Chrome, Cốc Cốc, Firefox).
   * Website đã được cấu hình chạy mượt mà trên giao thức tệp `file:///` lẫn máy chủ web.

2. **Chia sẻ cho người khác**:
   * Bạn có thể gửi file **`bundle.html`** cho bạn bè, phụ huynh hoặc giáo viên — file này chứa sẵn toàn bộ script & style bên trong nên chỉ cần 1 file duy nhất là có thể chạy ngay.

3. **Chạy qua Live Server (trong VS Code)**:
   * Mở thư mục này bằng VS Code.
   * Chuột phải vào `index.html` và chọn **Open with Live Server**.

---

## 🌟 Các tính năng chính

* **Thời Khóa Biểu Tuần**: Hiển thị trực quan theo thời lượng thực của tiết học, có thể bấm vào từng tiết để chỉnh sửa môn, phòng học, giáo viên, ghi chú.
* **Hôm Nay Học Gì?**: Dòng thời gian thông minh theo dõi các tiết học trong ngày, tự động phát sáng và đếm giờ tới tiết đang diễn ra.
* **Quản Lý Bài Tập Về Nhà**: Theo dõi bài tập theo môn, deadline, trạng thái hoàn thành với hiệu ứng confetti chúc mừng.
* **Quản Lý Môn Học**: Tùy chỉnh danh mục môn, tên viết tắt, mã màu nhận diện.
* **Hồ Sơ Đa Người Dùng**: Thêm và chuyển đổi giữa nhiều học sinh hoặc các lớp khác nhau.
* **Quét TKB từ Ảnh (AI OCR)**: Tải ảnh thời khóa biểu lên, hệ thống tự động nhận diện chữ tiếng Việt và tạo lịch học.
* **Xuất Ảnh & In Ấn**: Xuất ảnh chất lượng cao để chia sẻ qua Zalo/Facebook hoặc in ra giấy khổ A4 tiêu chuẩn.
* **Sao Lưu & Khôi Phục**: Hỗ trợ xuất/nhập tệp JSON và copy/paste chuỗi dữ liệu trực tiếp.
