# Mô phỏng hội thoại giữa hai Agent AI

## 🧠 Giới thiệu

Dự án này mô phỏng một cuộc trò chuyện giữa **hai agent AI** với khả năng trao đổi, phản hồi và hợp tác để thực hiện một tác vụ lập trình. Người dùng có thể tương tác thông qua một **giao diện trực quan** được xây dựng bằng **Gradio**.

Kết quả cuối cùng là đoạn mã được hai agent thống nhất tạo ra cùng với **kết quả thực thi** đoạn mã đó.

---

## 🗂 Cấu trúc dự án


### 📄 Chi tiết các file

- **`agent.py`**  
  Khởi tạo các agent với khả năng phản hồi theo ngữ cảnh. Mỗi agent có thể đóng vai trò khác nhau trong hội thoại.

- **`utils.py`**  
  Định nghĩa một class hỗ trợ xử lý đa luồng (threading) nhằm đảm bảo cuộc trò chuyện diễn ra liên tục và mượt mà.

- **`chat.py`**  
  Xây dựng hộp thoại cho phép hai agent tương tác qua lại. Sau hội thoại, chương trình sẽ **trích xuất đoạn mã được tạo ra** và **kết quả thực thi đoạn mã** đó.

- **`app.py`**  
  Tạo giao diện trực quan với **Gradio**, cho phép người dùng theo dõi cuộc hội thoại và xem kết quả mà hai agent đưa ra.

---

## 🚀 Cách chạy chương trình


```bash
pip install -r requirements.txt

python app.py

