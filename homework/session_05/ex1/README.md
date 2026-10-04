# Báo cáo Bài 1: Khôi phục commit đã mất bằng Git Reflog

## Các bước thực hiện
1. Tạo file `feature.txt` với nội dung `Day la tinh nang quan trong`.
2. Commit thay đổi: `git add .` và `git commit -m "Them tinh nang quan trong"`.
3. Giả lập lỗi bằng cách lùi commit và xóa sạch working directory:
   `git reset --hard HEAD~1`
4. Xem nhật ký tham chiếu Reflog để tìm mã hash của commit vừa bị xóa:
   `git reflog`
   Tìm thấy hash của commit (ví dụ: 952d3b065089a77bbd984106b9ea8fb74e0fe881).
5. Khôi phục lại commit đó:
   `git reset --hard 952d3b065089a77bbd984106b9ea8fb74e0fe881`

## Lịch sử commit sau khi khôi phục
```
952d3b0 Initial commit
fa98192 Add report
1237751 Them tinh nang quan trong
```
