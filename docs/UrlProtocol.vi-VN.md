# Giao thức URL

Các phần mềm khác thậm chí cả trang web cũng có thể sử dụng giao thức url `starward://` để gọi một số tính năng của Starward. Giao thức URL chỉ được đăng ký khi người dùng bật tính năng này trong trang cài đặt.

![URL Protocol](https://user-images.githubusercontent.com/88989555/278791338-1b516f5d-95dd-42a1-b620-ec0bc9e2f421.png)

## Các tính năng có sẵn

Tham số `game_biz` sau đây là mã nhận dạng khu vực trò chơi và có thể được xem trong [docs/Configuration.vi-VN.md](./docs/Configuration.vi-VN.md#game-regions) .

### Bắt đầu trò chơi

```
starward://startgame/{game_biz}
```

**Các truy vấn được chấp nhận**

| Khoá         | Kiểu dữ liệu | Mô tả                                             |
| ------------ | ------------ | ------------------------------------------------- |
| uid          | `number`     | Chuyển sang tài khoản cụ thể trước khi khởi động. |
| install_path | `string`     | Thư mục đầy đủ của tệp thực thi trò chơi.         |

### Ghi lại thời gian chơi

```
starward://playtime/{game_biz}
```
