# vscode_setting
for internal use.


## インストール

### 事前準備
githubの[アクセストークン](https://docs.github.com/ja/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)を取得してください。

1. githubにログインをしてください。
2. プロファイルの画像をクリックし、次に `Setting` をクリックしてください。
3. サイドバーで `Developer settings` をクリックしてください。
4. サイドバーで `Personal access token` の下にある `Fine-grained tokens` をクリックしてください。
5. `Generate new token` をクリックします。
6. `Token name` に任意のトークン名を入力します。 
   - その他の項目はそのままの状態で問題ないです。
7. `Generate token` をクリックします。
8. 生成されたアクセストークンをコピーします。
9. composerにアクセストークンを設定します。
   ```
   composer config --global github-oauth.github.com <access-token>
   ```

### 手順
1. 当リポジトリをクローンしてください。
   ```
   git clone git@github.com:pressmaninc/vscode_setting.git
   ```
2. 拡張機能から推奨される拡張機能をインストールしてください。
3. rootディレクトリでcomposerをインストールしてください。
   ```
   cd vscode_setting
   composer install
   ```
