# Tên Dự án 

## Mô tả
- Hệ thống gồm 3 đối tượng: Người mua view, Server, Trâu cày view. 
- Người mua view thông qua website sẽ đăng ký link cần cày, thời gian cày của link, (số điểm trâu sẽ nhận được),...  
- Server nhận link đó cung cấp cho các Trâu cày view, tính điểm cho Trâu cày.
- Trâu cày (client cài app windows) nhận link từ server, tùy theo yêu cầu chủ link mà cày.
## Kiến trúc

## Server 
### Các chức năng
- Cung cấp các API: 
    - Getlink: (mô tả API)
    - ...
## Client
### Các chức năng
- call API getlink, trả về khoảng X items 
- item gồm các thông tin:  Link, số giây, id
- client có thể chạy đồng thời 10 link hoặc theo thứ tự.
- client sẽ giám sát số điểm của mình, số link mình đã xử lý, thời gian xử lý mỗi link. 
- link sau khi được mở đến hết thời gian quy định sẽ đóng browser và gửi lên server id để nhận điểm. 
 
```diff
- (?)Lảm thế nào để biết được là client có thực hiện đúng yêu cầu của chủ link(?) 
```
        

- client đăng nhập