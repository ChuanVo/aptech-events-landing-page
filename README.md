# Hướng dẫn thực hành lập trình website Landing page cơ bản

## A. Cài đặt phần mềm
### 1. Visual studio code
#### 1.1 Window
- Link download (chọn hệ điều hành window)
https://code.visualstudio.com/
-  Hướng dẫn cài đặt
https://code.visualstudio.com/docs/setup/windows

#### 1.2 MacOS
- Link download (Chọn hệ điều hành MacOS)
https://code.visualstudio.com/

- Hướng dẫn cài đặt
https://code.visualstudio.com/docs/setup/mac


## B. Thực hành

#### 1. Tạo folder `aptech-landing-page` ở desktop

#### 2. Mở folder `aptech-landing-page` trong visual studio code
file -> Open Folder -> Chọn folder & OK

#### 3. Tải resource về máy 
1. [Download here](https://drive.google.com/drive/folders/1UqasgPZM6hCGg4XVgyNcNKf-DrH7gxiG?usp=drive_link ) 

2. Giải nén và copy 3 folder `css`, `img` và `js` và folder `aptech-landing-page`

#### 3. Tạo file index.html
![alt text](image-1.png)

#### 4. Khởi tạo code html
![alt text](image-2.png)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing-Page</title>
</head>
<body>
    <div class="container">
        Xin chào mọi người! chúc mọi người buổi tối vui vẻ!
    </div>
</body>
</html>
```

#### 5. Kiểm tra nội dung mới thêm vào
![alt text](image-3.png)

#### 6. Chỉnh sửa nội dung file html
1. Thêm code cho phần `home`
```html
<div id="home">
    <div class="content">
        <h1>Họ và Tên</h1>
        <h3>Mô tả về bản thân</h3>
        <a href="#about" class="btn btn-green">Khám phá thêm</a>
    </div>
</div>
```

2. Thêm code cho phần `about`
```html
<div id="about">
    <div class="content">
        <h5>Giới thiệu</h5>
        <h3>Sở thích</h3>
        <div class="list">
            <div class="list-item">
                <div class="caption">
                    <div class="caption-title">Cầu lông</div>
                    <div class="caption-content">Mô tả</div>
                </div>
                <img src="./img/so-thich-1.jpg">
            </div>
            <div class="list-item">
                <div class="caption">
                    <div class="caption-title">Bóng rổ</div>
                    <div class="caption-content">Mô tả</div>
                </div>
                <img src="./img/so-thich-2.jpg">
            </div>
            <div class="list-item">
                <div class="caption">
                    <div class="caption-title">Trekking</div>
                    <div class="caption-content">Mô tả</div>
                </div>
                <img src="./img/so-thich-3.jpg">
            </div>
            <div class="list-item">
                <div class="caption">
                    <div class="caption-title">Chụp ảnh</div>
                    <div class="caption-content">Mô tả</div>
                </div>
                <img src="./img/so-thich-4.jpg">
            </div>
        </div>
    </div>
</div>
```
3. Thêm code cho phần `map`
```html
<div id="map">
    <div class="content">
    <h3>Địa chỉ</h3>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3919.060333257187!2d106.71161431098558!3d10.806691158589564!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x317529ed00409f09%3A0x11f7708a5c77d777!2zQXB0ZWNoIENvbXB1dGVyIEVkdWNhdGlvbiAtIEjhu4cgVGjhu5FuZyDEkMOgbyB04bqhbyBM4bqtcCBUcsOsbmggVmnDqm4gUXXhu5FjIHThur8gQXB0ZWNo!5e0!3m2!1sen!2s!4v1729571181897!5m2!1sen!2s" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
</div>
```

4. Thêm code cho phần `footer`
```html
<div id="footer">
    <div class="content">
    <div class="list">
        <div class="row">
        <div class="cart">
            <i class="fa-brands fa-facebook-f"></i>
        </div>
        <div class="cart">
            <i class="fa-brands fa-twitter"></i>
        </div>
        <div class="cart">
            <i class="fa-brands fa-github"></i>
        </div>
        </div>
        <div class="row">
        <p>Copyright &copy; 2024 - HỆ THỐNG ĐÀO TẠO LẬP TRÌNH VIÊN QUỐC TẾ APTECH</p>
        </div>
    </div>
    </div>
</div>
```

#### 7. Thêm `css` cho trang web thêm sinh động
```html
  <link rel="icon" href="./img/favicon.ico">
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap">
  <link rel="stylesheet" href="./css/style.css">
  <link rel="stylesheet" href="./css/font-awesome.css">
```

![alt text](image.png)

#### 8. Thêm `menu` cho trang web
![alt text](image-5.png)
![alt text](image-4.png)

1. Thêm code cho phần `menu`
```html
<a href="#" class="btn-hamburger">
<i class="fa-solid fa-bars"></i>
</a>
<div class="menu-outside"></div>
<div class="menu">
<div class="menu-header">
    <span>Menu</span>
    <div class="btn-close">
    <i class="fa-solid fa-xmark"></i>
    </div>
</div>
<div class="menu-body">
    <ul class="sidebar">
    <li class="item"><a href="#home">Home</a></li>
    <li class="item"><a href="#about">About</a></li>
    <li class="item"><a href="#map">Map</a></li>
    <li class="item"><a href="#footer">Footer</a></li>
    </ul>
</div>
</div>
```

#### 9. Thêm code `js` để thao tác với trang web
```html
<script src="./js/script.js"></script>
```

#### 10. Bài tập
Hãy chỉnh sửa thông tin của trang web theo các yêu cầu sau:
1. Đổi thông tin: Họ và Tên -> Họ và tên của bạn
2. Đổi thông tin: Mô tả về bản thân -> Mô tả bản thân bạn
3. Đổi màu tên của bạn từ đen sang đỏ
4. Bấm vào nút `Khám phá thêm` đi đến `map`
