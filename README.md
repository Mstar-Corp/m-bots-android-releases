# M-Bots cho Android — bản phát hành

Repo này chỉ chứa file cài đặt (APK) của app M-Bots, không có mã nguồn.

- Tải bản mới nhất: mục **Releases** → bản trên cùng → `m-bots-<phiên bản>.apk`.
- App tự báo khi có bản mới: dòng "Có bản mới" hiện trên đầu màn hình chính, bấm vào là tải về và cài đè (giữ nguyên dữ liệu, không phải ghép nối lại).
- App chỉ dùng được khi đã ghép nối với máy chủ M-Bots của Mstar.

Mỗi release kèm `latest.json` mà app đọc để biết có bản mới:

```json
{"versionCode": 10506, "versionName": "1.5.6", "apkUrl": "https://github.com/…/m-bots-1.5.6.apk", "notes": "…"}
```

APK ký bằng khoá phát hành của Mstar Corp. SHA-256 chứng chỉ ký:
`548a2f7d1ddc6e9fa07f2d3c430d8780d598e3f059efd119574931a2c57edc65` (kiểm bằng `apksigner verify --print-certs`).
