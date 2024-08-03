# FastHTML dựa trên 3 nền tang chính: 

1. ASGI (Asynchronous Server Gateway Interface): Đơn giản hoá giao thức HTTP thành một API Python đơn giản. 

- ASGI nhằm xử lý các giao thức HTTP và WebSockets một cách không đồng bộ. 
- ASGI có thể được coi là "cầu nối" giữa máy chủ web và ứng dụng Python của bạn.

## Cách hoạt động của ASGI:

1. Chuyển đổi HTTP thành API Python:
- ASGI chuyển đổi các yêu cầu HTTP thành một cấu trúc dữ liệu đơn giản trong Python. 
- Một ứng dụng ASGI là một hàm Python nhận ba tham số: scope, receive, và send

2. Các tham số:
- scope: Thông tin về kết nối và yêu cầu, bao gồm loại giao thức, đường dẫn URL, headers, và hơn thế nữa.
- receive: Hàm không đồng bộ để nhận các sự kiện từ khách hàng (client).
- send: Hàm không đồng bộ để gửi các sự kiện đến khách hàng.