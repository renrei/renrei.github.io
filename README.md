🎀 NostrのNIP-05認証、GitHub Pagesでの取得方法をご紹介〜🎵

みんな〜、NostrのNIP-05認証を手に入れたいんだけど、どうやっていいかわからないよ〜って思っている人、れんれいが教えちゃうよ！✨

    🎤 とっても大事なお知らせ！: まずはGithubのアカウント持ってることが大前提なの❤️

🎉 れんれい流、簡単ステップ✨
1. さっそく、GitHubでリポジトリ作っちゃお！

    みんなの大好きなGitHubを開いてね
    右上の「+」ってところをポチッとな〜🖱️して、「New repository」を選んでね
    ここで大切なのは、リポジトリの名前を「ユーザ名.github.io」にすること！
        例えばrenreiだったら「renrei/renrei.github.io」みたいな感じかな🌟
    必ず公開設定（public）にして、「Create repository」ってボタンを押して進めちゃお！

2. _config.ymlファイル、作成タイム！📝

    できたてホヤホヤのリポジトリページに飛ぶよ

    「Add file」ってところをクリック！そこから「Create new file」を選んでね

    ファイルの名前は「_config.yml」にして、こんな感じで書いてね:

    yml

    include: [".well-known"]

3. ミステリアスなディレクトリ、.well-knownとnostr.jsonファイルを作ろう！

    再び「Add file」ってところをポチッとして、「Create new file」を選ぶよ

    ファイル名に「/.well-known/nostr.json」って入力するの

    そして、こんな風にnostr.jsonに書いてね:

    json

    {
      "names": {
        "_": "公開鍵をHex形式でここに入れちゃうyo"
      }
    }

    🚫 ちょっと待った！: 絶対に秘密鍵を公開しちゃダメだよ！大変なことになっちゃうからね！

4. nostr.jsonがちゃんと見れるか確認タイム🔍

    ちょっと待ってから、ブラウザで「https://ユーザ名.github.io/.well-known/nostr.json」を開いてみて
    ちゃんと自分の書いた内容が表示されているか確認してね！

5. 最後に、Nostrクライアントでピカピカに仕上げる✨

    Nostrクライアントを開いて
    NIP-05の欄に「_@ユーザ名.github.io」と入力して、さっと更新するの

🎤 これでばっちり！ あなたのGitHub PagesでのNIP-05認証、完璧に設定できたはずだよ！
