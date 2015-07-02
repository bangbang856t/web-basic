# web-basic
# Hướng dẫn
Đầu tiên các bạn fork về repo của mình, sau đó làm như sau

Click vào fork repo tại trang https://github.com/thanhnhan2tn/web-basic

Trên máy tính, bạn tạo một thư mục để lưu code trong quá trình học,
Vào thư mục tại máy của bạn Thao tác: mở CMD di chuyến đến thư mục chứa code, gõ vào lệnh
```
git clone https://github.com/taikhoancuaban/web-basic.git
git remote add web-basic https://github.com/thanhnhan2tn/web-basic.git
```
Sau khi clone về các bạn tạo branch training:
```
git checkout -b training
```

Và pull code từ training của repo web-basic về

```
git pull web-basic training
```

Mỗi task đều phải tạo 1 branch mới (không code trên training) ví dụ làm phần layout:

git checkout -b layout --> tạo branch layout

git rebase training --> đồng bộ code hiện tại với code từ repo training

Khi làm cần phải checkout sang training và pull code từ training của repo web-basic xem có bị thay đổi gì hay không, nếu có thì tiếp tục rebase và xử lý conflict sau đó push lên repo của mình

Gửi pull request:

Sau khi làm 1 task giả sử làm xong task layout: Add toàn bộ file đang làm vào staged

```
git add .
```

Commit
```
git commit -m "Nội dung comment"
```

Sau đó push code lên repo của bạn (không push lên web-basic nhé)

git push origin abc với abc là branch của task đang làm

Ở đây ví dụ bạn làm phần layout > thực hiện:
```
git push origin layout
```

Sau đó gửi pull request lên branch training của web-basic để so sánh và merge ([cần đọc document của git] (https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C6%A1-B%E1%BA%A3n-v%E1%BB%81-Git))

Lưu ý: Chỉ được gửi 1 commit / 1 pull request

