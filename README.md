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


