【初心者向け】Railsでメモ付きカレンダーを作ってみよう。 SimpleCalendar を参考に自分で作ってみました。 今まで学んできたことを思い出しながらそして、一つ一つ確認しながら、そして まだまだ技術が足りずにわからないことはネットで調べながら、作成しました。

難しかった点が最後の「SimpleCalendarのCSSを追加」の部分です。 app/assets/stylesheets/application.css /*　←ここを入れるのを忘れないことです。 *= require simple_calendar #こちらを追加 *= require_tree . *= require_self */

そして、必要なプラグインを追加しないと画面に表示されないので注意です！ $ yarn add @babel/plugin-proposal-private-methods @babel/plugin-proposal-private-property-in-object これは記載がなかったので、コーディング後起動させたら、Webpacker::Manifest::MissingEntryErrorが出ました。 なので必要なプラグインの追加は忘れずに。

参照サイト： 【初心者向け】Railsでメモ付きカレンダーを作ってみよう。SimpleCalendar https://zenn.dev/yuma_rails/articles/00b6ea10b87ca5 【Rails6】Webpacker::Manifest::MissingEntryErrorを解決する https://qiita.com/ginger-yell/items/8584e9149496940ea144