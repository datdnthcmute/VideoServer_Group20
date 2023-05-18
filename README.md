# VideoServer_Group20 
[HTTP API video server](https://github.com/datdnthcmute/VideoServer_Group20) nhóm 20  
Link source code tham khảo: https://github.com/superdesk/video-server

<b><i>GVHD: TS. Huỳnh Xuân Phụng</i></b>
## Thành viên nhóm
- Nguyễn Thị Bích Liên - 20110335
- Đặng Nguyễn Thiên Đạt - 20110629

## **Ngôn ngữ sử dụng**
- Python

## **Môi trường**
_Cài đặt môi trường theo yêu cầu của các version sau_
- Python (>=3.6)
- FFmpeg
- MongoDB
- RabbitMQ

## **Cài đặt để phát triển**
**_LƯU Ý: Sử dụng virtualenv và pip để cài đặt các module python._**
Tại thư mục ta setup code

> **git clone https://github.com/superdesk/video-server.git**

Cài đặt máy chủ video để phát triển
LƯU Ý: virtualenv của bạn phải được kích hoạt

> **pip install -e video-server/[dev]**

## **Chạy máy chủ video để phát triển**
_Máy chủ video bao gồm hai phần chính: http api và celery workers._

Để bắt đầu một máy chủ http api dev:

1. Đặt biến env `FLASK_ENV` để phát triển trên Windows:

> set FLASK_ENV=developement

2. Chạy `python -m videoserver.app`

## Chạy với Docker
 
#### Sử dụng Docker-compose

Đầu tiên sử dụng git clone đồ án của nhóm về:
```sh
git clone https://github.com/datdnthcmute/VideoServer_Group20
cd VideoServer_Group20
```
Tiến hành chạy docker-compose để tạo container:
```sh
docker-compose up -d
```


> Lưu ý:  
 Khi chạy với docker compose mọi yêu cầu dịch vụ như trên FFmpeg, MongoDB, RabbitMQ sẽ không được yêu cầu tải trên localhost mà sẽ được tải tự động vào container của docker.


### Superdesk

Bản quyền thuộc về Superdesk việc sử dụng ở đây chỉ dành cho mục đích học tập 

To use a video-server with a [Superdesk](https://github.com/superdesk/superdesk-core) see the [docs](https://github.com/superdesk/superdesk-core/blob/develop/docs/video_server.rst)

