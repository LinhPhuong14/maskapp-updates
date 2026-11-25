# maskapp – kho cập nhật

Thư mục này chứa **gói cập nhật đã ký** (chuẩn TUF) của maskapp, do CI của repo chính tự đẩy lên.
Không có mã nguồn hay dữ liệu người dùng.

- `windows-x64/`: metadata TUF (`root.json`, `targets.json`, `snapshot.json`, `timestamp.json`)
  và gói `maskapp-<phiên bản>.tar.gz` / `.patch`.
- App chỉ cài bản cập nhật khi chữ ký khớp `root.json` đóng gói sẵn trong bộ cài, nên nơi chứa
  file này không cần được tin cậy.
- Không sửa tay, không xoá file cũ: client cũ cần metadata và patch của các bản trước.
