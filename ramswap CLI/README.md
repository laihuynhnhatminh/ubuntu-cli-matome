# RAMSWAP CLI

## Tạo một file swap mới

```bash
sudo fallocate -l 1G /swapfile
```

## Thiết lập quyền truy cập cho file swap

```bash
sudo chmod 600 /swapfile
```

## Đánh dấu file là một không gian swap

```bash
sudo mkswap /swapfile
```

## Kích hoạt swap file

```bash
sudo swapon /swapfile
```

## Mở file /etc/fstab để dán đoạn này vào `/swapfile swap swap defaults 0 0`

```bash
sudo nano /etc/fstab
```

## Xác nhận swap đã được kích hoạt

```bash
sudo swapon --show
sudo free -h
```
