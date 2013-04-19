Tí Sửu Client
=============

Tí Sửu client: Plugin cho ứng dụng web, mobile với 1 dòng mã script duy nhất


Dạng chatbox nổi trên Website, các tham số sử dụng mặc định
=============

```bash
<script type="text/javascript" src="http://www.manlab.vn/chat/bot-id?type=ajax&lang=vi"></script>
```

## Tham số:
- bot-id: mã định danh robot của bạn đã đăng ký và khởi tạo trên: www.manlab.vn
- type = ajax: mặc định load dữ liệu không đồng bộ
- lang = vi: sử dụng ngôn ngữ tiếng việt cho robot


Dạng chatbox tùy chỉnh trên Website
=============

```bash
<script type="text/javascript" src="http://www.manlab.vn/chat/bot-id?type=ajax&lang=vi&app=web&msg=id1&send=id2&log=id3&max=6"></script>
```

## Tham số:
- bot-id: mã định danh robot của bạn đã đăng ký và khởi tạo trên: www.manlab.vn
- type = ajax: mặc định load dữ liệu không đồng bộ
- lang = vi: sử dụng ngôn ngữ tiếng việt cho robot
- app = web (mặc định)
- msg = id1: id box nội dung chat
- send = id2: id button gửi nội dụng chat
- log = id3: id box lưu hội thoại chat
- max = 6: số bản ghi lịch sử chat được hiển thị, mặc định hiện thị tất nếu ko được đưa ra hoặc max <= 0

Dạng chatbox tùy chỉnh trên ứng dụng mobile
=============

```bash
<script type="text/javascript" src="http://www.manlab.vn/chat/bot-id?type=ajax&lang=vi&app=mobile&msg=id1&send=id2&log=id3&max=6"></script>
```

## Tham số:
- bot-id: mã định danh robot của bạn đã đăng ký và khởi tạo trên: www.manlab.vn
- type = ajax: mặc định load dữ liệu không đồng bộ
- lang = vi: sử dụng ngôn ngữ tiếng việt cho robot
- app = web (mặc định)
- msg = id1: id box nội dung chat
- send = id2: id button gửi nội dụng chat
- log = id3: id box lưu hội thoại chat
- max = 6: số bản ghi lịch sử chat được hiển thị, mặc định hiện thị tất nếu ko được đưa ra hoặc max <= 0


Nâng cao, viết lại plugin
=============
Bạn hoàn toàn có thể tự viết lại api cho ứng dụng thông qua lập trình socket.io, bằng việc request để lấy thông tin của server dưới dạng mã json trả về. Tham khảo source, thư mục src

## Request
```bash
http://www.manlab.vn/get/api?plugin=custom
```

## Response
```bash
{
  server : "http://chat.server-name.com:2013/chat"
}
```

