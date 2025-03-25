# 📲 Push Notifications without Google Services

> Hướng dẫn thiết lập **push notification** cho Z-Chat (Matrix client) **mà không cần Firebase/Google Services**, dành cho các hệ thống độc lập, bảo mật hoặc muốn tuỳ biến cao.

---

## 🧱 Kiến trúc tổng quan

Z-Chat sử dụng nền **Matrix** và có thể tích hợp với hệ thống push riêng qua:
- `Sygnal` (Matrix Push Gateway)
- `UnifiedPush` (cho Android không dùng Firebase)
- `matrix-pushgateway` (như [matrix_hedwig](https://github.com/element-hq/pushgateway))

---

## ✅ Các bước cấu hình

### 1. 🎯 Chọn cơ chế push

Bạn có thể chọn 1 trong 2:

| Phương án | Dùng cho | Ghi chú |
|----------|-----------|--------|
| **Sygnal** + Push Gateway | Cả iOS & Android | Cần cấu hình chi tiết |
| **UnifiedPush** | Android (LineageOS, GrapheneOS, /e/, v.v.) | Không dùng Google hoàn toàn |

---

### 2. 🔧 Cấu hình Sygnal (Matrix Push Gateway)

1. Cài đặt [Sygnal](https://github.com/matrix-org/sygnal)

```bash
git clone https://github.com/matrix-org/sygnal
cd sygnal
pip install -r requirements.txt
