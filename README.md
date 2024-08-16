# Windows PCを新しく購入したときに行うこと
## 設定･ソフトウェアインストール
- Flow Launcher
- WSL2
    - https://qiita.com/MinadukiSekina/items/25f3440565ca7b6a359e
- Rust
    - 原則Dev Container以外でRustは書かないが，cargoコマンドを使えるようにするため
    - exa
        - lsの代わり
        ```
        // cのコンパイラが必要
        sudo apt-get update
        sudo apt install -y build-essential
        cargo intall exa --locked
        ```
    - bat
        - catの代わり
        ```
        cargo install bat --locked
        ```
    - snippet
        - cargo-snippetで自動生成
- ~/.bashrsの編集
    - 好みのaliasやRUST_HOMEを設定
- starshipのインストール
    ```
    curl -sS https://starship.rs/install.sh | sh
    ```
    - bashを修飾する
- Linuxコマンド
    - unzip 
    ```
    sudo apt install unzip
    ```
    - tree
    ```
    sudo apt install tree
    ```
- Google Drive
    - Windows側のフォルダを同期
- Cursor
    - settings.json
    - rust.json
- Docker Desktop for Windows
    - もしかしたらdockerコマンドが権限で使えないかもしれないので、以下のようにdocker.sockの権限を変更する [参考](https://qiita.com/Nw3965/items/8e75da0012cb7a451cc2)
    ```
    > ll /var/run/docker.sock
    srw-rw---- 0 root 16 Aug 19:12 /var/run/docker.sock

    > sudo chmod 666 /var/run/docker.sock
    > ll /var/run/docker.sock
    srw-rw-rw- 0 root 16 Aug 19:12 /var/run/docker.sock
    ```
- Commit Mono
- mac-precision-touchpad
- 英字配列化
- Google日本語入力
    - ctrl + spaceで変換できるように
    - かな入力時も半角数字等を出したい
    - https://raspi.ryo.sc/google_ime_ctrl_space_onoff/
- Zotero
- MS Office
    - 大学のライセンス
    - ppt
        - テンプレートをコピーしてくる
- Brave
    - デバイス間の同期設定でブックマークや拡張機能，パスワードを引き継ぐ
- Slack
- Discord
- システム音声のオフ