# 1. Git基本操作編

## 準備
- Gitインストール
- バージョンの確認: `$ git --versions`
- エディタの登録
	- VS Codeの場合: `$ git config --global core.editor "code --wait"`
- ユーザー登録
	- `$ git config --global user.name "rockyhg"`
	- `$ git config --global user.email "hrk.haga@gmail.com"`
- SSHアクセス設定
- VS Code 拡張機能
	- Git Graph
	- Markdown All in One

## 基本操作編
- ディレクトリ作成 `markdown-template`
- VS Codeで上記ディレクトリを開く
- ターミナル (Git Bash) を起動
- Gitを初期化する
	- `git init`
	- VS Code: 「Initialize Repository」ボタン
	- 「init」は「initialize（初期化する）」の略
	- カレントディレクトリがワークツリーとして設定される
	- カレントディレクトリに「.git」というディレクトリが作成される
- ファイル「sample.md」を新規作成する
- MarkDownで記述
	- 見出し
	- リスト
	- リンク
	- 画像
- ステージングエリアに追加する
	- `$ git add sample.md`
	- VS Code: +ボタン
- ステージングエリアに入っているファイルのリストを表示する
	- `$ git ls-files`
	- 「ls-files」は「list files」の略
- ステージングエリアにあるファイルやディレクトリを、 ローカルリポジトリにコミットする
	- `$ git commit -m "Message"`
	- VS Code: Commitボタン
	- 「-m」は「message」の略
	- 「-m」オプションを指定しないで単に「git commit」すると、設定されたエディタが開いて、エディタ上でコミットメッセージの入力ができるようになる
- コミットの履歴を表示する
	- `$ git log`
	- VS Code: Git Graphボタン
- ワークツリーとステージングエリアの差分を表示する
	- `$ git diff`
	- VS Code: ファイルを選択する
