---
layout: post
title: RegionalRubyKaigi レポート (TODO) 松江 Ruby 会議 09
short_title: RegionalRubyKaigi レポート (TODO) 松江 Ruby 会議 09
tags: 0058 MatsueRubyKaigi09Report
---
{% include base.html %}


## RegionalRubyKaigi レポート 松江 Ruby 会議 09

### はじめに

2018年6月30日（土）に松江Ruby会議09が開催されました。今年は合計50名の方々に参加いただきました。

* 日時：2018年6月30日（土）11:00〜17:30（懇親会: 18:00〜）
* 場所：松江オープンソースラボ
* 主催：Matsue.rb（まつえるびー）
* 後援：日本Rubyの会
* 動画による中継(Youtube)：[https://www.youtube.com/watch?v=Q4QBVKDZwcg](https://www.youtube.com/watch?v=Q4QBVKDZwcg)
* Togetterまとめ： [https://togetter.com/li/1243152](https://togetter.com/li/1243152)
* 公式タグ・Twitter：[#matrk09](https://twitter.com/hashtag/matrk09)

![01_all.jpg](TODO.jpg)

### 島根でRubyが使えるようになったキッカケ (ゲスト講演)

* 発表者
  * 井上 浩氏([@NaCl](https://twitter.com/nacl))

![02_guest01_inoue.jpg](./02_guest01_inoue.jpg)

TODO: @sho-h

### TODO (基調講演)

* 発表者
  * まつもとゆきひろ氏([@yukihiro_matz](https://twitter.com/yukihiro_matz))

![03_keynote_matz.jpg](TODO.jpg)

TODO: @nishidayuya

### Redmineの更新を楽にする？1つの方法

* 発表者
  * 橋本 将氏([@sho_hashimoto](https://twitter.com/sho_hashimoto))
* 資料
  * [https://www.slideshare.net/shohashimoto/redmine1-103850531](https://www.slideshare.net/shohashimoto/redmine1-103850531)

![03_session1_sho-h.jpg](TODO.jpg)

TODO: @tomo-k

### 僕とMastodon

* 発表者
  * 平岡 瞬氏([@S_H_](https://gamelinks007.net/@S_H_))
* 資料
  * [https://speakerdeck.com/gamelinks007/pu-tomastodon](https://speakerdeck.com/gamelinks007/pu-tomastodon)

![04_session2_s_h_.jpg](./04_session2_s_h_.jpg)

山陰で稼働しているMastodonインスタンスの1つであるいわみどんを運営されている平岡氏にMastodonの最近の動向を紹介いただきました。PWA対応のような機能的なお話からじゃんけんに負けたらアカウントが凍結されるというインスタンスのお話まで幅広く紹介いただきました。今後の課題としてアカウントの削除による連合の負荷のような実際に起きうる問題まで把握されていたのが印象的でした。

また、平岡氏が開発したプロダクトを紹介していただきました。以下はその一部ですが、Togetterや氏のスライドに他のものも掲載されていますので是非ご覧ください。

* [Foods Checker](https://github.com/S-H-GAMELINKS/FoodsChecker): Mastodonアカウントでログインできる食品管理サービス
* [Legion](https://github.com/S-H-GAMELINKS/Legion): Ruby/Tk製のMastodonクライアント

### LTセッション

きむらしのぶ氏([@mix_dvd](https://github.com/mix_dvd))の司会で以下の4件のLTの発表が行われました。

* 松江ではたらく
  * 発表者
    * 加藤 龍氏([@k0matatsu](https://twitter.com/k0matatsu))

* 僕たちとRuby
  * 発表者
    * ハー・タイン 氏 & ポール 氏

* わたしとスプラウト.rb
  * 発表者
    * 竹田 喜世子氏

* Rubyでつくるスレッド
  * 発表者
    * 前田 修吾氏
  * 資料
    * [https://www.slideshare.net/ShugoMaeda/ruby-103693472](https://www.slideshare.net/ShugoMaeda/ruby-103693472)

### 若手エンジニア × Rubyプロジェクト = ？？？

* 発表者
  * 石川 瑞希氏

![05_session3_ishikawa.jpg](TODO.jpg)

TODO: @tomo-k

### 後方互換の保ち方

* 発表者
  * 日高 克也氏([@hidakatsuya](https://twitter.com/hidakatsuya))
* 資料
  * [https://speakerdeck.com/hidakatsuya/how-to-maintain-compatibility](https://speakerdeck.com/hidakatsuya/how-to-maintain-compatibility)

![06_session4_hidaka.jpg](./06_session4_hidaka.jpg)

日高氏が開発しているThinreportsを0.8から0.9にバージョンアップした時の変更を例として「後方互換の保ち方」についてお話いただきました。
Thinreportsのtlfファイル内に保存されたデータにあるsvgは、0.8はそのまま文字列として保存されていましたが、開発時に差分が確認しにくいなどの不便な点があり、0.9ではJSON形式で保存するように変更されたとのことでした。
単純に0.9でJSON形式に変更しただけでは、0.8のtlfファイルが読み込めなくなるので、0.9で0.8のtlfファイルを使用する時は、0.9のJSON形式で変換してから読み込めるように変更されたとのことでした。
上記のような後方互換の保ち方を修正箇所のコード付きでご説明いただき、公開したプロダクトをバージョンアップした時にどのような点を気にすべきか共有していただいたセッションでした。あと今後のThinreportsの新機能についてもご紹介いただきました。

* [Thinreports](http://www.thinreports.org/)

### Yet Another Ruby Application Framework "Alone"

* 発表者
  * 東 裕人氏（TOC しまねソフト研究開発センター）

![07_session5_higashi.jpg](./07_session5_higashi.jpg)

東氏がOSSとして公開している「Alone」について活用事例の紹介を含めてお話ししていただきました。
事例の紹介の際には実際にどのようなコードで動いているかなどの解説もあり、会場の関心を集めていました。
コードを含めた詳しい説明をしていただいたおかげで、わかりやすく、大変有意義なセッションとなりました。

**「Alone」**
http://www.ruby-alone.org/

### Ruby Quiz

* 発表者
  * 倉橋 徹氏([@torukurahashi](https://twitter.com/torukurahashi))と竹田 喜世子氏
* 資料
  * [https://github.com/matsuerb/matrk/blob/master/09/ruby-quiz.md](https://github.com/matsuerb/matrk/blob/master/09/ruby-quiz.md)

![08_rubyquiz.jpg](TODO.jpg)

TODO: @nishidayuya

## 謝辞

### ご協力いただいた企業様

[エクスウェア株式会社](https://www.xware.co.jp/), [ファーエンドテクノロジー株式会社](https://www.farend.co.jp), [株式会社ネットワーク応用通信研究所](http://www.netlab.jp/), [株式会社Misoca](https://www.misoca.jp), [株式会社イーストバック](http://www.eastback.co.jp/)

## 著者について

### 西田 雄也 ([@nishidayuya](https://twitter.com/nishidayuya))

プログラマ。
Redmineは職場ではもちろん、結婚式のタスク管理以降、家族でも使っている。
2014-12に [redmine_text_format_converter](https://github.com/nishidayuya/redmine_text_format_converter) というプラグインを開発し、Redmineの書式をTextileからMarkdownに変換して管理下の全てのプロジェクトをMarkdownへ移行させました。

### 佐田 明弘 ([@sada4](https://twitter.com/sada4))

Matsue.rbにひっそりといるプログラマ。

### 吉岡 隆行 ([@yoshioka_cb](https://twitter.com/yoshioka_cb))

コミュニティー（勉強会）おじさん。松江Ruby会議09 実行委員長。

### 木村 友哉([@tomo-k](https://github.com/tomo-k))

Apple 信者な Rubyist。

### 橋本 将 ([@sho_hashimoto](https://twitter.com/sho_hashimoto))

Matsue.rb の雑用係。[定例会](http://matsue.rubyist.net/about_us/#matsuerb)にはだいたい出席してます。
