# Báo cáo Bài 1: Khôi phục commit đã mất bằng Git Reflog

## Các bước thực hiện
1. Tạo file `feature.txt` với nội dung `Day la tinh nang quan trong`.
2. Commit thay đổi: `git add .` và `git commit -m "Them tinh nang quan trong"`.
3. Giả lập lỗi bằng cách lùi commit:
   `git reset --hard HEAD~1`
4. Xem nhật ký tham chiếu Reflog để tìm mã hash của commit vừa bị xóa:
   `git reflog`
   Tìm thấy hash của commit (ví dụ: 10e8412d9ffb1ebd3791a09e384daf8fbe4e951d).
5. Khôi phục lại commit đó:
   `git reset --hard 10e8412d9ffb1ebd3791a09e384daf8fbe4e951d`

## Lịch sử commit sau khi khôi phục
```
10e8412 Add report
952d3b0 Initial commit
fa98192 Add report
1237751 Them tinh nang quan trong
```
