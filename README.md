# 💌 Tháng Mười Dịu Dàng

Món quà nhỏ 20/10 gửi người thương: một trang web tĩnh với giọt sương kéo giãn rồi nở thành đóa hoa, kèm tấm thiệp chúc ở giữa.

## Xem trang

```
[https://<tên-github>.github.io/<tên-repo>/index.html](https://nguyennhan209.github.io/thang-muoi-diu-dang/)
```

Thay `<tên-github>` và `<tên-repo>` bằng tên của bạn. Vì file là `main.html` (không phải `index.html`), link **phải có `/main.html`** ở cuối, nếu không sẽ bị lỗi 404.

## Đổi tên người nhận bằng link

Thêm `?` và các tham số sau tên file:

| Tham số | Ý nghĩa | Mặc định |
| --- | --- | --- |
| `ten` (hoặc `name`) | Tên người nhận | `Min iu` |
| `tu` (hoặc `from`) | Tên người gửi, hiện ở cuối thiệp | `Anh` |
| `loichuc` | Lời chúc riêng trong thiệp | Lời chúc có sẵn |

Ví dụ:

```
main.html?ten=Linh
main.html?ten=Linh&tu=Nam
main.html?ten=Linh&tu=Nam&loichuc=Cảm ơn em đã ở bên anh
```

Giới hạn độ dài: `ten` 45 ký tự, `tu` 30 ký tự, `loichuc` 320 ký tự. Ký tự điều khiển bị loại bỏ và nội dung được escape trước khi hiển thị.

## Công nghệ

HTML, Tailwind CSS (Play CDN), JavaScript thuần, SVG và Canvas. Không cần build, không có backend.

> Tailwind Play CDN phù hợp trang nhỏ như thế này. Nếu muốn tối ưu tốc độ tải thì nên chuyển sang CSS đã build sẵn.
