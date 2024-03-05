# 1. Git基本操作編

## 準備
- Gitインストール
- バージョンの確認:
  - `git --versions`
- エディタの登録
	- VS Codeの場合:<br>
  	`git config --global core.editor "code --wait"`
- ユーザー登録
	- `git config --global user.name "xxx"`
	- `git config --global user.email "xxx@example.com"`
- VS Code 拡張機能
	- Git Graph
	- Markdown All in One

## 基本操作編
- ディレクトリ作成
  -  `markdown-template`
- VS Codeで上記ディレクトリを開く
- ターミナル (Git Bash) を起動する
- Gitを初期化する
	- Git Bash: `git init`
	- VS Code: 「Initialize Repository」ボタン
	- カレントディレクトリがワークツリーとして設定される
	- カレントディレクトリに「.git」というディレクトリが作成される（隠しファイル扱いのため普段は見えない）
- ファイル「sample.md」を新規作成する
- MarkDownで記述
	- 見出し
	- リスト
	- リンク
	- 画像
- ステージングエリアに追加する
	- Git Bash: `git add sample.md`
	- VS Code: +ボタン
- ステージングエリアにあるファイルやディレクトリを、 ローカルリポジトリにコミットする
	- Git Bash: `git commit -m "Message"`
	- VS Code: Commitボタン
- コミットの履歴を表示する
	- Git Bash: `git log`
	- VS Code: Git Graphボタン
- ワークツリーとステージングエリアの差分を表示する
	- Git Bash: `git diff`
	- VS Code: ファイルを選択する
