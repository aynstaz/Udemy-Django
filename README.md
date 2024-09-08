# Udemy-Django

- Git の使い方・手順

  1. 最新の develop ブランチをロードする
     ```
     git fetch
     git pull origin develop
     ```
  2. 最新の develop から作業用ブランチ（feature/AAA）を作成する
     ```
     git checkout -b feature/AAA
     git branch <- 現在操作中のブランチを確認する
     ```
  3. ファイルを更新（開発）する
  4. 更新した内容をセーブする
     ```
     git add . <- 更新した（作成した）ファイル全てをコミット対象とするコマンド
     git commit -m "コミット内容を説明するメッセージ"
     ```
  5. セーブした（コミットした）内容をリモート環境へ反映（Push）する
     ```
     git push origin feature/AAA
     ```
  6. 開発した内容をマージしてもらうリクエストを作成する
     - Pull Request など
  7. リクエストのレビュー完了後、マージする
  8. 上記マージ後の最新 develop ブランチをローカルに読み込む<br>※ まだ develop ブランチ自体は最新化されていない
     ```
     git fetch
     ```
  9. ローカルの develop ブランチを最新化すべく、develop ブランチへ移動し最新の内容を反映させる
     ```
     git checkout develop
     git pull
     ```
  10. 機能の開発時は都度 feature/AAA を作成する<br>手順２へ戻る
