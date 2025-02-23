# Ubuntu interaction with Firewall CLI

## Kiểm tra trạng thái tường lửa (nếu bật thì sẽ show port mở)

```bash
sudo ufw status
```

## Bật tường lửa, nhưng cái này chỉ bật trong phiên làm việc hiện tại thôi, reboot là nó tự tắt

```bash
sudo ufw enable
```

## Yêu cầu tường lửa lên mỗi khi khởi động lại server

```bash
sudo systemctl enable ufw
```

## Mở port 22 (ssh), Nginx Full mở rồi không cần mở lại

```bash
sudo ufw allow ssh
```

## Mở port 3000

```bash
sudo ufw allow 3000
```

## restart ubuntu

```bash
sudo reboot
```

## Đóng port 4000

```bash
sudo ufw delete allow 4000
```
