---
title: SE備忘録 2021年下期
date: 2022-04-18
categories: 技術
tags: [diary]
---
システムエンジニアに就いて2年が経った。2021年下期を振り返る。

- [SE備忘録 2020年上期](https://tech.hukurouo.com/articles/2020-10-20-se-hurikaeri1)
- [SE備忘録 2020年下期](https://tech.hukurouo.com/articles/2021-04-20-sehurikaeri2)
- [SE備忘録 2021年上期](https://tech.hukurouo.com/articles/2021-10-17-sehurikaeri3)

## 会社でやったこと

### 広告掲載管理システムの開発

- Rails + GoogleAdManagerAPI でウェブ広告掲載を管理するアプリ
- メイン開発は自分一人なので、伸び伸びと開発できた
- おまかな方針は立っていたので、それをロジックに落とし込んで実装していった
- とりあえず動かせる状態に持っていき、開発環境に反映させて運用チームに実際に触ってもらうことを心がけた
  - やりたいことが技術的に可能かどうかを確かめることができた
  - 実際に動かしてみると分かる改善点もたくさんあった
- 広告運用チームが持っていたドメイン知識を得ることに苦労した
  - 少人数で回していることもあり、属人化の傾向が強かった
  - MTGを定期的に開催し、新しく入った人もそれを見れば全体像が理解できるように、ドキュメントに適宜まとめていった
  - 技術側からも機能の改善案など提案ができるようになった　運用チーム視点と開発視点の双方向から設計を考えていくことができた
  - 何のための機能なのか、そもそもこれは必要な機能なのか、業務フローのほうで改善できまいか、というところを考えることができるようになった

### CFnでインフラ構築

- 2021年下期は主にインフラ方面を中心に学習した
- 学習内容のアウトプットとして Zenn に本を書いた
  - https://zenn.dev/hukurouo/books/cfn-hands-on
- インフラは面白い
  - バックエンドと同じくらい面白いな～という気持ちがある
  - Kubernetes とかも触ってみたい

### 設計がんばる
- 中規模の Rails アプリを1から設計して実装していく初めての経験
- Rails はその名前の通りレールに沿っていれば大丈夫という感じだったので、とにかく Rails の規約に沿うことを心がけた
- とはいえクラス設計など悩むところは結構あったので、設計の本をいくつか読んだ
  - このあたりの知識は色々なところに活かせそうなので、もうちょっと踏み込もうと思っている
  - 2022年上期は設計を主にやっていきたい

### OSS にコントリビューションをした
- 会社で使っている OSS ライブラリにいくつかPRを送った
- example コードの不備を発見したのがきっかけ
- 本当に些細な修正だったので、勇気を出してはじめてのコントリビューションを試みた
  - https://github.com/googleads/google-api-ads-ruby/pull/184
  - https://github.com/googleads/google-api-ads-ruby/pull/185
- 無事にマージされる
- 大分自分の中で敷居が下がり、結構気軽にPRを送れるようになった
  - https://github.com/googleads/google-api-ads-ruby/pull/186
  - https://github.com/prawnpdf/prawn/pull/1265

## 趣味でやったこと

2021年下期は AtCoder に夢中だった。最終的に緑コーダーになれた。

https://atcoder.jp/users/hukurouo

半年ほどやって大分満足した。上のほうでも書いたけど設計周りをしっかり勉強したかったので、一旦競プロはやめることにした。

## 読んだ本

#### ドメイン駆動設計入門 ボトムアップでわかる! ドメイン駆動設計の基本

DDD についてざっくりと理解したかったので読んだ。かっちりと設計したいなら、こういう風になるのだな～と思った。読みやすく変更しやすい設計とは、をとにかく丁寧に説明している本だった。

#### オブジェクト指向設計実践ガイド ~Rubyでわかる 進化しつづける柔軟なアプリケーションの育て方

かなり良い本。設計に正解はなく、最善を目指してやっていくしかないみたいなことが書いてあり、なるほどと思った。これは多分何回か読み直すと思う。

#### メタプログラミングRuby

Ruby の仕組みを解説する本。Ruby ではすべてがオブジェクトであるということが良く分かった。Ruby はとても柔軟な言語で、本当にいろいろな記述ができる。黒魔術的なテクもいくつか紹介されていたけど、そういった記述は可読性とのトレードオフだと思っているので、業務では書けないな～と思いつつ流し読んだ。

#### AWSコンテナ設計・構築[本格]入門

ECS Fargate 周りを勉強するために買った本。入門としては本当にこの一冊で良いのでは？と思うほど良い本だった。やっぱり手を動かして勉強できるハンズオン形式の書籍は良いですね。

