# Mini guideline — bài làm cá nhân

> Điền nội dung này trước khi bắt đầu gán nhãn. Giữ lại các quyết định sau khi self-QC.

## Định nghĩa lớp

| Lớp | Định nghĩa của bạn | Ví dụ/điểm phân biệt |
| --- | --- | --- |
| `car` | Xe con, sedan, hatchback, SUV, CUV, xe taxi, xe bán tải| Xe từ 4-9 chỗ ngồi hoặc bán tải cỡ nhỏ|
| `truck` |Xe tải chở hàng, xe đầu kéo, xe cứu hộ/cẩu tải, xe tải thùng lớn/nhỏ | Có phần thùng chở hàng riêng biệt phía sau hoặc kết cấu khung cẩu/chở hàng chuyên dụng|
| `bus` |Xe buýt công cộng, xe khách cỡ lớn/trung, xe buýt 2 tầng |Xe chở nhiều hành khách, thân xe dài, nhiều cửa kính hông dọc thân |
| `van` |Xe van chở hàng, minivan, xe khoang kín chuyên chở người/hàng hóa |Thân xe dạng khối hộp liền mạch (không tách cabin/thùng như truck), nhỏ hơn bus nhưng cao hơn car |

## Quy tắc chung

- Box bám sát vật thể nghĩa là: Ôm vừa sát phần thân xe thực tế nhìn thấy được, không bao gồm khoảng trống, mặt đường hay bóng đổ.
- Vật thể bị che khuất: Vẽ box quanh toàn bộ phần thân xe còn nhìn thấy được nếu vẫn xác định được đúng lớp xe.
- Vật thể bị cắt bởi rìa ảnh: Vẽ box chạm đúng mép ảnh quanh phần thân xe xuất hiện trong khung hình; không tự đoán phần nằm ngoài ảnh.
- Vật thể rất nhỏ/mơ hồ: Xe ở xa quá mờ hoặc xe máy/người đi bộ/biển quảng cáo thì không gán nhãn

## Ghi lại quyết định cho ít nhất ba ca mơ hồ

| Ảnh | Tình huống | Quyết định cuối | Lý do theo schema |
| --- | --- | --- | --- |
| `drive_017` |Hàng xe đỗ/nối đuôi ở xa bên mép đường phải |Gán nhãn từng xe dạng car / van cho các xe rõ shape; bỏ qua cụm quá mờ |Xe đang đỗ vẫn phải gán nhãn theo đúng loại xe; giữ nguyên tắc ôm sát phần nhìn thấy |
| `drive_042` |Xe tải chở đống hàng cồng kềnh chở quá khổ phía sau | Gán nhãn truck ôm cả cabin và phần thùng chở hàng (không bao gồm phần hàng chìa ra ngoài quá xa nếu mờ)| Vật thể chính là xe tải chở hàng truck; box ưu tiên ôm sát kết cấu xe và hàng gắn liền.|
| `drive_046` | Xe cứu hộ/cẩu giao thông (công an) màu trắng ở giữa đường| Gán nhãn truckĐây là xe chuyên dụng có cabin và sàn/cẩu phía sau, thuộc phân loại xe tải/xe chuyên dụng truck, không phải car hay van. (ID: 1)| |
