
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
git branch -d [branch_test]
```
[branch_test] 削除します。

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

```
branch -m [古いブランチ名] [新しいブランチ名]
```
古いブランチ名を[新しいブランチ名]に変更する
```
git branch -m [新しいブランチ名]
```
現在の作業中のブランチを変更する

### ローカルに保存されてるプロジェクトをGithubにプッシュする
- GithubでREADMEがないリポシトリンを新規作成する
![alt text](https://github.com/voiceJapan/TrainningGuide/blob/master/Git/gitRepo.png "github repo Readme")
- ロカールプロジェクトディレクトリに入って、下記のコンマンドラインを実行する
```
git init
git add README.md
git commit -m "first commit"
git remote add origin [github_repository_url]
git push -u origin master

```
- [github_repository_url]
![alt text](https://github.com/voiceJapan/TrainningGuide/blob/master/Git/repoURL.png "repo URL")

### Pull request
- プルリクエストとは、簡単に言うと、「ソースコードを変更、追加しましたのでのでreviewしてもらえますか。問題がなければ、Masterにマージお願いします。」と言うメッセンジーをmaster  リポジトリの管理者に送る。

#### Github flow(フロー)
![alt text](https://github.com/voiceJapan/TrainningGuide/blob/master/Git/githubFlow.png "github flow")
- https://guides.github.com/introduction/flow/
- 1. ブランチを作成する
- 2. コミット追加する
- 3. プルリクエストを作成する
- 4. ソースコードreview
- 5. デイプロい



