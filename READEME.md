# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
- リモートリポジトリはプロジェクトのコードやファイルを複数の開発者が、変更内容を共有・同期する
  オンラインの保管場所。
- ローカルリポジトリ開発者個人のローカルPC上に保存する保管場所のこと。


## プッシュとマージの違いは何でしょうか？
- プッシュは、ローカル環境で行った変更をリモートリポジトリにアップロードする操作のこと。
- マージは異なるブランチの変更を統合する操作のこと。


## コミットとプッシュの違い
- コミットはローカルリモートリポジトリに変更を保存したいときに行う
- プッシュはコミットでローカルに変更を確定させた後、リモートリポジトリに送信して反映させる操作


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
- 変更内容がわかるように記載する。
- prefix機能を使用して分かりやすくする。
  - prefixについて
    1. feat: 新しい機能の追加を示す
    2. fix: バグ修正を示す
    3. docs: ドキュメントの変更を示す
    4. style: コードスタイルの変更（フォーマット、セミコロンの追加など）を示す...etc


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
- ローカルでマージするフロー
  1. リモートリポジトリからコードを取得、もしくはinitで新しくローカルにリポジトリを作成
  2. 修正等の変更が完了したら、ローカルブランチに変更をコミットする。
  3. リモートブランチ、masterに変更をプッシュ

- プルリクエストでのマージするフロー
  1. リモートリポジトリからコードをプル。もしくはinitで新しくローカルにリポジトリを作成
  2. 修正等の変更が完了したら、ローカルブランチに変更をコミットする。
  3. リモートリポジトリにプッシュ
  4. プルリクを変更内容を記載して作成
  5. プルリクエスト上でコードレビューをしてもらう
  6. コードレビューが完了してプルリクエスト承認してもらいマージ許可
  7. 上司がマージする
  8. リモートリポジトリに変更内容が反映される。


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
  コンフリクトを起こした部分を担当しているエンジニアに相談してどう修正するかを相談して
  変更点を最終的にどう反映させるかを話し合う。またチームメンバーや上司にも相談して、最終的に
  どう変更していくかをチームで話し合って決める。
