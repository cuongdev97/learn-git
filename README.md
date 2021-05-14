1. git init
2. git status
3. git add
    3.1. use "git restore --staged <file>..." to unstage => Dùng để hủy lệnh add, đưa file về ra khỏi vùng staged
    3.2. use "git restore <file>..." to discard changes in working 
directory: Khi file chưa được add mà ở trạng thái modified đỏ thì lệnh này đưa nội dung về lúc chưa modified
4. git commit
5. git log / git log --oneline
6. git show <id commit>
    Nếu có nhiều thay đổi thì phải bấm phím xuống nhiều lần mới hiện ra hết. Sau đó bấm q để quit
7. git diff 
    Dùng để xem thay đổi của các file khi vừa sửa và chưa có add vào staged

8. working directory
9. staging area
10. git repository

11. git checkout    
    git checkout -- <file>: tương tự git restore ở 3.2

12. git reset
    git reset HEAD <file>: tương tự 3.1

13. git checkout -b <branch>
    tạo 1 branch mới và checkout vào đó

14. git branch <branch>
    tạo 1 branch mới

15. git checkout <branch>
    checkout vào branch đó

16. git merge
    kéo thay đổi từ branch này vào branch khác
    VD: kéo thay đổi từ branch feature sang branch main
        + Bước 1: git checkout main (đảm bảo đang ở branch cần nhận thay đổi)
        + Bước 2: git merge feature (gộp thay đổ từ feature vào main)
    
17. git branch -D <branch> : Xóa branch

18. git reset --soft <id_commit>
    id_commit là id lần commit phía trước của HEAD
    => HEAD trỏ về lần commit trước và các thay đổi vẫn được giữ ở staging area (modifed xanh chờ để commit)

19. git reset --mixed <id_commit>
    => HEAD trỏ về lần commit trước và các thay đổi vẫn được giữ nhưng bị bỏ ra khỏi staging area (modifed đỏ chờ để add)

20. git reset --hard <id_commit>
    => Xóa bỏ tất cả các commit phía trên của commit đó
    => dùng cẩn thận


