# Treasure Date Map 💗

Mini project HTML/CSS/JS thuần để deploy trực tiếp bằng GitHub Pages.

## Chạy local

Chỉ cần mở `index.html` trong trình duyệt.

## Deploy GitHub Pages

1. Tạo repository mới trên GitHub, ví dụ `date-adventure`.
2. Upload `index.html` vào root của repo.
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**.
5. Branch: `main`, folder: `/ (root)`.
6. Save. Sau ít phút trang sẽ ở dạng `https://username.github.io/date-adventure/`.

## Đổi nội dung

Trong `index.html`, tìm:

```js
const stops = [ ... ];
```

Mỗi stop có:
- `x`, `y`: vị trí % trên bản đồ
- `time`: giờ
- `title`: tên checkpoint
- `note`: lời nhắn / nhiệm vụ funny

## Dùng ảnh mặt 2 người

Tạo thư mục `images/`, ví dụ:

```text
images/me.jpg
images/her.jpg
```

Rồi đổi:

```js
const couple = {
  you: { initials: "ME", image: "images/me.jpg" },
  partner: { initials: "U", image: "images/her.jpg" }
};
```

Ảnh sẽ tự crop thành icon nửa mặt trái + nửa mặt phải ở mỗi checkpoint.
