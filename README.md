# photo-business-app

燃費とガソリン代を計算する、iPhone Safari対応の小さなWebアプリです。

## できること

- 走行距離からガソリン代を計算
- 車に表示される燃費 `km/L` で計算
- `L/100km` 表示にも対応
- ガソリン単価ごとの比較表示
- 台数を入れて合計費用を計算
- iPhoneのホーム画面に追加してアプリのように起動

## 計算式

```text
必要なガソリン量 = 走行距離 ÷ 燃費
1台あたりの費用 = 必要なガソリン量 × ガソリン単価
合計費用 = 1台あたりの費用 × 台数
```

例:

```text
120km ÷ 12km/L = 10L
10L × 180円/L = 1,800円
```

## ファイル構成

```text
index.html          アプリ本体
manifest.json       iPhone/スマホ向けWebアプリ設定
service-worker.js   オフライン表示用キャッシュ
icon.svg            ホーム画面用アイコン
README.md           この説明書
```

## GitHub Pagesで公開する方法

1. GitHubでこのリポジトリを開く

   ```text
   https://github.com/ungorenge2-bit/photo-business-app
   ```

2. 上部メニューの `Settings` を開く

3. 左メニューの `Pages` を開く

4. `Build and deployment` の `Source` を `Deploy from a branch` にする

5. `Branch` を次のように設定する

   ```text
   main / root
   ```

6. `Save` を押す

7. 数十秒から数分待つ

8. 公開URLを開く

   ```text
   https://ungorenge2-bit.github.io/photo-business-app/
   ```

## iPhoneで使う方法

1. iPhoneのSafariで次のURLを開く

   ```text
   https://ungorenge2-bit.github.io/photo-business-app/
   ```

2. 画面下の共有ボタンを押す

3. `ホーム画面に追加` を押す

4. 名前を `燃費計算` のまま追加する

5. ホーム画面のアイコンから起動する

## 注意

- `file:///tmp/...` のようなMac内の一時ファイルURLは、iPhoneでは開けません。
- iPhoneで使うには、GitHub PagesなどでWeb公開された `https://...` のURLをSafariで開いてください。
- GitHub Pagesを有効にした直後は、公開URLが反映されるまで少し時間がかかることがあります。
