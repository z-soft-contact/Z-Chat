# 🔐 Hướng dẫn sử dụng mã hóa đầu cuối (E2EE) trong Z-Chat

Mã hóa đầu cuối (End-to-End Encryption - E2EE) là cơ chế bảo mật giúp **chỉ người gửi và người nhận** mới có thể đọc được nội dung tin nhắn.  
Không ai – kể cả máy chủ, quản trị viên hệ thống hoặc bên thứ ba – có thể truy cập nội dung đã mã hóa.

---

## ✅ Lợi ích khi sử dụng E2EE

- 🛡️ Bảo mật tối đa nội dung trò chuyện
- 🔐 Tin nhắn chỉ giải mã được trên thiết bị chính chủ
- 🧩 Không lo bị rò rỉ dữ liệu dù server bị tấn công

---

## 🧭 Cách hoạt động của E2EE trong Z-Chat

- Khi bạn tham gia phòng chat có E2EE, thiết bị của bạn sẽ **tạo cặp khóa riêng (public/private)**
- Tin nhắn sẽ được mã hóa bằng **khóa công khai (public key)** của người nhận trước khi gửi
- Chỉ thiết bị có **khóa riêng (private key)** mới có thể giải mã tin nhắn
- Nếu bạn đăng nhập trên thiết bị mới, bạn cần xác minh lại (verify) để lấy quyền giải mã

---

## 🧪 Cách sử dụng E2EE trong Z-Chat

### 1. 🔒 Kiểm tra trạng thái phòng chat
- Trong giao diện phòng chat, biểu tượng 🔐 trên đầu phòng cho biết phòng đã được mã hóa đầu cuối hay chưa

### 2. ✅ Bật xác minh thiết bị (nếu được yêu cầu)
- Khi đăng nhập trên thiết bị mới, bạn có thể cần xác minh danh tính để đảm bảo bạn là chủ tài khoản
- Xác minh bằng cách:
  - So sánh mã bảo mật giữa hai thiết bị
  - Duyệt xác minh bằng mã QR hoặc mã số

### 3. 🔁 Đồng bộ khóa
- Z-Chat hỗ trợ tính năng **backup và khôi phục khóa mã hóa** nếu bạn muốn dùng nhiều thiết bị
- Vào phần **Cài đặt → Bảo mật → Sao lưu khóa**, nhập mật khẩu bảo vệ để tạo bản sao an toàn

---

## 📌 Lưu ý quan trọng

- Nếu bạn **mất khóa riêng (private key)** và không sao lưu, bạn **sẽ không thể đọc lại tin nhắn cũ**
- Hãy **bật tính năng sao lưu khóa** để tránh mất dữ liệu

---

## ❓ Câu hỏi thường gặp

### Q: Tôi thấy phòng chat không hiển thị biểu tượng 🔐?
- A: Phòng chat đó chưa được bật mã hóa. Hiện tại, Z-Chat hỗ trợ mã hóa cho các phòng riêng (private rooms) và nhắn tin cá nhân.

### Q: Tôi không thể đọc tin nhắn sau khi cài lại máy?
- A: Bạn cần **khôi phục khóa mã hóa** đã sao lưu trước đó hoặc nhờ thiết bị cũ xác minh lại.

---

## 📬 Hỗ trợ

Nếu bạn cần hỗ trợ thêm, vui lòng liên hệ:

- 📧 Email: support@z-cloud.com.vn
- 🌐 Website: [https://z-soft.com.vn](https://z-soft.com.vn) / [https://z-cloud.com.vn](https://z-cloud.com.vn)

---

**Z-Chat – Bảo mật cuộc trò chuyện của bạn, từng tin nhắn.**
