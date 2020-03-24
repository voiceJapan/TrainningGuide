
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

#### 1.Thao tác với Repository
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
git add  file_name
```
add 1 file đã thay đổi

```
git add . 
git add *.*
```
add toàn bộ thay đổi
```
git commit 
```
tạo snapshots nhưng thay đổi tại local repository
```
git commit -m "comment"
```
commit và add message xem nội dung commit là gì
```
git push
```
cập nhật các thay đổi từ local lên remote
```
git status
```
kiểm tra trạng thái hiện tại của local repository

```
git diff
```
xem nội dung của file đã thay đổi

#### 2.Thao tác với log

```
git log
```
xem toàn bộ các thay đổi đã thực hiện
```
git log --decorate --graph --oneline
```
```
git log --graph --oneline --all
```
```
git log --pretty=format:"%h %s" --graph
```

#### 3.Thao tác với branch
mỗi người 1 branch, mỗi task 1 branck, mỗi bug 1 branch
```
git branch
```
xem toàn bộ các branch hiện có
```
git branch -d branch_name
```
xoá branch 

```
git branch branch_name
```
tạo branch mới

```
git checkout -b branch_name
```
tạo branch mới và di chuyển sang branch mới

```
git merge
```
merge branch khác vào branch hiện tại.

###  Đưa 1 project có sẵn lên github
- tạo repo ko kèm file readme
- di chuyển vào thư mục project, chạy command line theo hướng dẫn github

### Pull request
- Không phải ai cũng có quyền merge source vào remote master 
- Hướng dẫn cách tạo pull request, cách comment pull request.
- Đơn giản chỉ là: Ê code nè, merge giùm đi
- Giúp commit ngắn gọn hơn
- Hỗ trợ code review, ngăn code ẩu

