# M-Bots cho Android — bản phát hành

Repo này chỉ chứa file cài đặt (APK) của app M-Bots, không có mã nguồn.

- Tải bản mới nhất: mục **Releases** → bản trên cùng → `m-bots-<phiên bản>.apk`.
- App tự báo khi có bản mới (từ 1.5.7): thông báo trên điện thoại nếu đang không mở app, và dòng "Có bản mới" trên đầu màn hình chính. Bấm "Cập nhật" là app tự tải, kiểm tra SHA-256 rồi mở trình cài của Android; cài đè, giữ nguyên dữ liệu và ghép nối. Lần đầu Android hỏi cho phép M-Bots cài ứng dụng: bật lên rồi quay lại, app tự cài tiếp.
- App chỉ dùng được khi đã ghép nối với máy chủ M-Bots của Mstar.

Mỗi release kèm `latest.json` mà app đọc để biết có bản mới:

```json
{"versionCode": 10508, "versionName": "1.5.8", "apkUrl": "https://github.com/…/m-bots-1.5.8.apk", "notes": "…", "sha256": "<SHA-256 của APK>"}
```

APK ký bằng khoá phát hành của Mstar Corp. SHA-256 chứng chỉ ký:
`548a2f7d1ddc6e9fa07f2d3c430d8780d598e3f059efd119574931a2c57edc65` (kiểm bằng `apksigner verify --print-certs`).
