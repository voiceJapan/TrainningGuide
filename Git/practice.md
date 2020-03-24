
## バージョン管理とGit

### バージョン管理システム　（Version Control System）
- ファイルの変更を管理するものです。
- ソースコードの変更を管理するシステム
- 同じソースコードに対して複数人が同時に作業をサポートするシステム
- ソースコードを別バージョンに戻すシステム。

### Git
- Gitに限らずですが、分散バージョン管理システムで重要なのは「リポジトリ」という概念です。このリポジトリに全てのファイルの変更履歴が管理されています。
- Gitのメイン概念：
	+ Repository (リポジトリ)
	+ Branch （ブランチ）：ブランチとは、履歴の流れを分岐して記録していくためのものです
	+ Pull Request (プルリクエスト)
	+ Commit
	+ Push, pull
	+ Merge

#### install Git
- https://git-scm.com/download (window/mac/Linux/Unix)

## Github
- GitHubは、Gitの仕組みを利用して、世界中の人々が自分の作品(プログラムコードやデザインデータなど)を保存、公開することができるようにしたウェブサービスの名称です。
- Gitのウェブサーバー。

### Githubコマンドのご紹介

#### 1.Repositoryに関するコマンド
```
 git init
```
リポジトリを新規に作成する
```
 git clone
```
義tふbに保存されてるリモートのリポジトリ(ファイルやディレクトリの状態)をロカールコピーする
```
 git pull
```
リモートのリポジトリの内容をローカルのリポジトリに取り込む
```
git push
```
ローカルのリポジトリの内容をリモートのリポジトリに送り込む
```
git add  file_name
```
作業ブランチにある一つのファイルの更新内容を、インデックスに反映する
```
git add . 
git add *.*
```
作業ブランチにある全部ファイルの更新内容を、インデックスに反映する
```
git commit 
```
追加・変更したファイルをGitに登録する

```
git commit -m 「comment」
```
コミットしながら、説明のメッセンジーをコミットに追加する
```
git status
```
ワーキング・ツリーの状態を表示する

```
git diff 「ダイレクトリー」
```
ファイルの変更内容を表す
working tree と index の差分などを表示する

#### 2.ロッグに関するコマンド

```
git log
```
```
git log --decorate --graph --oneline
```
```
git log --graph --oneline --all
```
```
git log --pretty=format:"%h %s" --graph
```

#### 3.Branch（ブランチ）に関するコマンド
 「注意」タスク、バッグに対しては、それぞれブランチを作成してください。

```
git branch
```

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


alooo

