# Security Policy

## Phạm vi

Repository này chỉ là **kho lưu trữ phát hành tĩnh (static release storage)** cho ứng dụng **SYSCORE**. Nó không chứa mã nguồn của ứng dụng — mã nguồn được lưu trữ riêng tại một repository private.

Chính sách bảo mật dưới đây áp dụng cho:
- Tính toàn vẹn của các file phát hành (`.exe`, `.blockmap`, `latest.yml`) được đăng tại [Releases](https://github.com/hoangvantuan123/syscore-releases/releases).
- Quy trình cập nhật tự động (auto-update) của ứng dụng.

## Các phiên bản được hỗ trợ

| Phiên bản       | Được hỗ trợ        |
| --------------- | ------------------ |
| Mới nhất (Latest) | ✅                 |
| Các bản cũ hơn   | ❌                 |

Chỉ phiên bản mới nhất trong mục Releases được vá lỗi bảo mật. Người dùng nên luôn cập nhật lên bản mới nhất qua cơ chế auto-update trong ứng dụng.

## Báo cáo lỗ hổng bảo mật

Nếu bạn phát hiện vấn đề bảo mật (ví dụ: file cài đặt bị giả mạo, sai lệch SHA-512 trong `latest.yml`, hoặc lỗ hổng trong cơ chế cập nhật), vui lòng **không** tạo issue công khai. Thay vào đó, hãy báo cáo riêng tư bằng cách:

- Gửi email trực tiếp cho quản trị viên repository, hoặc
- Sử dụng mục **Security** → **Report a vulnerability** trên trang GitHub của repository này.

Chúng tôi sẽ phản hồi trong thời gian sớm nhất có thể và giữ kín thông tin cho đến khi có bản vá chính thức.

## Xác minh tính toàn vẹn bản phát hành

Mỗi bản phát hành đi kèm file `latest.yml` chứa mã băm **SHA-512** của bộ cài đặt. Trước khi cài đặt thủ công, bạn có thể tự đối chiếu mã băm này với file `.exe` đã tải về để đảm bảo file không bị chỉnh sửa trong quá trình phân phối.
