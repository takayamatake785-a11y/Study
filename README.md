# Study Quest v1.0

iPhoneで使えるPWA（ホーム画面に追加できるWebアプリ）のソースです。

## 含まれる機能
- XP・レベル
- クエストの追加と達成
- 自由学習報告と強度/理解度に応じたXP計算
- ゲーム/アニメ/動画などの報酬ショップ
- 学習履歴・交換履歴
- JSONバックアップと復元
- localStorageによる端末内保存
- オフライン用Service Worker

## 公開方法（GitHub Pagesの例）
1. GitHubで新しいリポジトリを作成（Public）。
2. このZIPを展開し、中のファイル一式をリポジトリ直下にアップロード。
3. リポジトリの Settings → Pages を開く。
4. Build and deployment の Source を「Deploy from a branch」にし、Branchを「main」、Folderを「/(root)」にしてSave。
5. 公開された `https://ユーザー名.github.io/リポジトリ名/` をiPhoneのSafariで開く。
6. Safariの共有ボタン →「ホーム画面に追加」→「追加」。

## データについて
記録はブラウザのlocalStorageに保存されます。同じiPhone・同じブラウザの同じサイトURLで使うことが前提です。SafariのWebサイトデータ消去、ブラウザ変更、端末変更などで消える可能性があります。定期的に「データ管理」からJSONバックアップを保存してください。

## 更新方法
1. 新機能や修正を `index.html` などに反映。
2. 変更したファイルをGitHubリポジトリに上書きアップロード。
3. Service Workerのキャッシュ名を変更（例：study-quest-v2）して再公開。
4. iPhoneでアプリを再読み込み。必要ならホーム画面アプリを一度終了して開き直す。

※この版はローカル端末内保存で、複数端末同期・アカウントログイン・クラウド保存は未実装です。
