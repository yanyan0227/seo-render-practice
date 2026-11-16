# Render SEO 練習サイト

## 1. GitHubに公開用リポジトリを用意
GitHubで新しいリポジトリ（例: seo-render-practice）を作り、このフォルダ内の `index.html` と `robots.txt` をアップロードしてください。`sitemap.xml.template` は準備用です。

## 2. Renderに公開
Render → New → Static Site → GitHubリポジトリを選択。
- Build Command: `echo 'Ready'`
- Publish Directory: `.`
- サイト名は利用可能な任意の名前

## 3. 公開URLが確定したら
`sitemap.xml.template` 内の `https://YOUR-SITE.onrender.com/` を、Renderで確定した正しいURLへ置換し、ファイル名を `sitemap.xml` として保存・アップロード。
`robots.txt` に `Sitemap: https://確定したホスト名.onrender.com/sitemap.xml` を追記。
新しいコミットでRenderが再公開されることを確認してください。

## 4. Google Search Console
https://search.google.com/search-console/ の「URLプレフィックス」で `https://確定したホスト名.onrender.com/` を追加。HTMLタグ方式なら提示された meta タグを index.html の <head> 内に入れて再公開し、所有権確認を行ってください。確認用タグは削除せず残します。

## 5. 登録・検証
Search Console の URL検査でトップURLを調べてインデックス登録をリクエスト。サイトマップ画面で `sitemap.xml` を送信。
数日から数週間かかることもあります。掲載は保証されません。

## 注意
- Render の Static Site を選択（Web Serviceとは区別）
- Googleビジネスプロフィールに架空の事業を登録しない
- この一式にはDNS/独自ドメイン設定は必要ありません
