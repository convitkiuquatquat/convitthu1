# Giới thiệu:
Đây là một repository được fork lại từ [https://github.com/truongvi02/v2heroku](https://github.com/truongvi02/v2heroku) với chức năng là tạo ra một server để vào mạng miễn phí.

Heroku sẽ không khuyến khích việc này nên các bạn cần phải fork lại dự án này để không bị heroku chặn.

Với nhu cầu không quá cao thì heroku chính là giải pháp hoàn hảo cho anh em muốn dùng 4G miễn phí:
* 2TB mỗi tháng
* 550 giờ mỗi tháng (~23 ngày, dĩ nhiên bạn cần ngủ 8 tiếng 1 ngày nên 550 giờ là quá đủ)

## Tổng quan

Dự án này phải được sử dụng một cách hợp lý nếu không sẽ bị chặn

Sau khi triển khai, mỗi khi khởi động sẽ tải bản mới nhất

## Triển khai

### Bắt đầu

 1. Fork dự án này đến tài khoản GitHub của bạn（trên PC có thể thấy nút Fork trên cùng bên tay phải, ví dụ tài khoản của bạn tên là `example`）
 2. Đổi lại tên dự án thành tên bất kỳ（Ví dụ đổi thành `demo`）
 3. Chỉnh sửa file `README.md`，đường dẫn `convitkiuquatquat/convitthu1` bằng đường dẫn của bạn（ví dụ `example/demo`）

> [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/convitkiuquatquat/convitthu1)

 4. Quay lại trang chủ của dự án，bấm vào liên kết để triển khai

### Đối số

Các đối số sẽ dùng trong quá trình cài đặt。

| Đối số | Mặc định | Diễn giải |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess user ID |
| `AID` | `64` | AlterID，Số từ 0 đến 65535 |
| `WSPATH` | `/` | |

## Truy cập CloudFlare

Hai phương pháp sau có thể kết nối ứng dụng với CloudFlare, từ đó tăng tốc độ ở một mức độ nhất định:

1. Liên kết tên miền với ứng dụng và kết nối tên miền với CloudFlare
2. Reverse proxy thông qua CloudFlare worker 

## Lưu ý

 1. ** Xin đừng lạm dụng dự án này, có rất ít dịch vụ miễn phí như Heroku, hãy sử dụng và trân trọng **
 2. Nếu bạn sử dụng tên miền để kết nối với CloudFlare, vui lòng xem xét bật TLS 1.3 
 3. Hầu hết các địa chỉ AWS IPv4 đã bị Twitter chặn 
