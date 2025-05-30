# コードレビューガイドライン

このリポジトリのコードレビューを円滑かつ効果的に行うためのガイドラインです。
現在はDevinのPRに関するガイドラインのみ掲載されていますが、将来的に他の内容も追記する予定です。


# レビューの基本方針
**完璧を求めるよりも、全体としての改善を優先してください。**
レビュー担当者は、PRが完全でなくとも、システム全体のコード健全性が確実に向上するならば、承認を優先してください。

ただし、以下のようなケースは改善を求めることができます。
* 不要な機能が実装されている
* 明らかに可読性の低いコードが実装されている
* 追加機能に関するテストが実装されていない

以下のような場合は、完璧ではなくともマージすることを検討してください。
* 最適な実装・設計ではないが、十分に動作するコードが実装されている

デザイン用のサブIssueはレビュー担当者の判断でCloseして開発フェーズに移行できます。
* 開発フェーズで実現性に問題があると発覚した場合は適宜デザインフェーズに戻ります

---

# DevinのPRについて
* [Devin](https://devin.ai/)が作成したPRについては、Devinのトリガーを引いた人（起動者）が動作確認を行ってください
    * 動作確認や修正に時間がかかりそうな場合は、起動者がその旨をgithub上にコメントしてください
* DevinのPRの承認とマージはDevinの起動者が行っても構いません
  * 必要に応じて、他のメンテナーをレビュワーに追加してください
    * e.g. フロントエンド側の機能をDevinに実装してもらったが、トリガーを引いた人のフロントの知識が浅い場合など
  * メンテナーは、レビュアーに追加されるまでDevinのPRは確認する必要はありません
