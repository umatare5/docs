# ソフトウェア・エンジニアリングとは何か

## 時間と変化

- コードには事実上無限の想定稼働時間 (保守稼働時間) を持つものがある
  - これは、組織の主力プロダクト、組織自体のプロダクト等が該当する
- 想定稼働時間が未知ということは、保守稼働時間も予想出来ない

  - このようなコードの持続可能性に投資しないことはリスクである
    - 想定稼働時間の長いコードではアップグレードが必要になる
      - アップグレードは以下の性質を持つ
        - 時間経過により、未知の前提条件や課題を含む
        - 人の変化により、担当者が未経験の場合が多い
        - 往々にして数年単位でまとめて実行され、単体の負荷が高い
      - アップグレードを経験した組織は以下を選択する
        - アップグレード自体を行わずフルリファクタする
        - アップグレードを定期的に行い、負荷を最小化する
          - Google は後者を選択している
        - 「何もしない」状態はありえない
          - これは Heartbleed や Meltdown, Spectre を回避しないことを意味する
  - 理論上理解していることと、正確な方法・それにかかる費用を実践上知っているということは別物である
  - プラクティスと専門知識は、効率と信頼性を大いに推進する。

## コスト管理

- 以下全てを考慮する。
  - 財務コスト (例：資金)
  - 資源コスト (例：CPU 時間)
  - 人件コスト (例：エンジニアリング能力)
  - 処理コスト (例：行動を取る場合にどんなコストがかかるか)
  - 機会コスト (例：行動を取らない場合にどんなコストがかかるか)
  - 社会コスト (この選択が社会全体にどのような影響を与えるか)
- 人間故のバイアスも考慮する。(現状維持バイアス、損失嫌悪バイアス等)