## Nội dung học
- Tìm hiểu sơ về Version Control, Git & Github
- Cài đặt Git trên máy

- Cơ bản: Tạo Github Repository, Git & Github
- Pull & push
- Cho các dự án đơn giản

- Nâng cao: Branch, Merge
- Confilict Resolving, Pull Request
- Cho các dự án lớn hoặc đi làm

## Git là gì
### Version Control
- Hệ thống giúp lưu trữ mọi thay đổi của source code
- Hỗ trợ nhiều người làm việc cùng lúc.
- Xem đứa nào thay đổi code.
- Revert các thay đổi, đưa code về version cũ hơn, không lo mất code

### Git
- Ra đời 2005, tác giả Linux Torvald
- Toàn bộ code và history được lưu trữ trên máy người dùng

#### Cơ chế hoạt động
- Repository: Là 1 collection của code, có thể lưu trên máy local hoặc remote server. Clone từ remote server: mang tất cả source code, thông tin trên remote về local. Cập nhật thay đổi từ remote về local-> pull, cập nhật thay đổi từ local lên remote->push.
- Snapshots: bản lưu trữ của tất cả các tác động với code, có thể come back lại các snapshots trước. Mỗi lần commits thì sẽ tạo 1 snapshots.
- Commit
- Branch

#### install Git
- https://git-scm.com/download (window/mac/Linux/Unix)

## Github

- Git remote server 

### Các lệnh Github cơ bản:
```
 git init
```
tạo ra 1 repossitory github
```
 git clone
```
clone 1 repository từ github về local
```
 git pull
```
cập nhật thay đổi từ remote repository về local.
```
git add và git add .
```
```
git commit 
```
tạo snapshots nhưng thay đổi tại local repository
```
git commit -m "comment"
```

```
git push
```

```
git log
```
```
git log -decorate -graph -oneline
```



