# BÃ¡o cÃ¡o BÃ i 1: KhÃ´i phá»¥c commit Ä‘Ã£ máº¥t báº±ng Git Reflog

## CÃ¡c bÆ°á»›c thá»±c hiá»‡n
1. Táº¡o file `feature.txt` vá»›i ná»™i dung `Day la tinh nang quan trong`.
2. Commit thay Ä‘á»•i: `git add .` vÃ  `git commit -m "Them tinh nang quan trong"`.
3. Giáº£ láº­p lá»—i báº±ng cÃ¡ch lÃ¹i commit vÃ  xÃ³a sáº¡ch working directory:
   `git reset --hard HEAD~1`
4. Xem nháº­t kÃ½ tham chiáº¿u Reflog Ä‘á»ƒ tÃ¬m mÃ£ hash cá»§a commit vá»«a bá»‹ xÃ³a:
   `git reflog`
   TÃ¬m tháº¥y hash cá»§a commit (vÃ­ dá»¥: `12377513a45f9880c7149b11b6c0ed68b3490154`).
5. KhÃ´i phá»¥c láº¡i commit Ä‘Ã³:
   `git reset --hard 12377513a45f9880c7149b11b6c0ed68b3490154`

## Lá»‹ch sá»­ commit sau khi khÃ´i phá»¥c
```
1237751 Them tinh nang quan trong
```
