# ToDo

Sorry, Japanese Only. [meme]

Flask本家のExampleに入っているminitwitのできが良いのでforkしてるもの。

- SQLite3からMariaDBへ移行
- Gravatar依存をなくして、自前のアイコン編集・ホスティングを準備 (croppieというOSSが良さそう)
- デザイン刷新、Mobile/Desktop 両対応へ (人気CSSフレームワークを使うと良さそう) 
- Emailで認証可能にする (またはEmailなしまたは確認なしEmailにしてSMSのあれで行けるかも)
- アカウント情報閲覧・設定ページを作る
- 通知機能
- FavとRT機能
- minitwit/templates/timeline.html が、public timeline (←全てのツイートを時系列)とmy timeline (←自分がフォローしたユーザーのツイートの時系列)と自分のタイムラインの3つをまとめて書いていて分かりにくい。分離するべきだと思う。(→public_timeline.html my_timeline.html, user_timeline あたりに)
- passwordをsha256ではなくsalt+hash形式へ変更

## Done

- password hashをsha1からsha256へ変更 (参考: https://security.googleblog.com/2017/02/announcing-first-sha1-collision.html) (sha256も将来的にはだめなのだろうか、ならsha3の方がよいかも)
- CSRFトークンを追加する

## Not to implement

