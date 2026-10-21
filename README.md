# Cờ Gánh Online

Cấu trúc cần có ở thư mục gốc repository:
```
server.py
requirements.txt
render.yaml
static/index.html
```

## Render
- Root Directory để trống khi các file trên nằm ở gốc repository.
- Build Command: `pip install -r requirements.txt`
- Start Command: `uvicorn server:app --host 0.0.0.0 --port $PORT`
- Commit tất cả file rồi chọn Manual Deploy → Deploy latest commit.

## Kiểm tra sau deploy
- `/health` phải trả JSON có status `ok`.
- `/version` phải trả build `2026-10-21-C`.

Có chơi online qua mã phòng, đấu máy 3 cấp độ, bảng điểm, lịch sử, ván mới, trang chủ, thoát game và hướng dẫn luật. Phòng lưu trong bộ nhớ tiến trình; nếu Render restart, phòng đang chơi sẽ mất. Đây là bản một instance để thử nghiệm.
