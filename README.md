# Address Mapper with GSI (AMwG)

Address Mapper with GSI (AMwG)は、地理院地図を利用して住所を地図上にプロットできるウェブベースのツールです。ユーザーフレンドリーで高機能に設計されており、自治体事業やまちづくりなど様々な用途に活用できます。AMwGはGNU General Public License v3.0の下で配布されており、自由にカスタマイズが可能です。

## 開発の経緯

厚生労働省のサイトで労災指定医療機関を検索した際、テキストで羅列させるという、とってもユーザーフレンドリーな設計だったので、このツールを作成しました。このツールを使えば、施設名と住所から簡単に地図上にプロットし、視覚的に確認できるようになります。元々はOpenStreetmap対応で開発していましたが、OSMのサーバー負荷を考慮して、地理院地図対応に変更しています。

## 特徴

- 地理院地図とジオコーディングサービスを使用して複数の住所を地図上にプロット(サーバーに負荷をかけないようデフォルトでは一件毎に200msの遅延をかけています)
- CSVインポート機能（古いバージョンのExcelに対応できるようShift-JISエンコーディングのみ）
- プロットされたすべての場所に合うように、地図のズームを自動調整
- シンプルで直感的なユーザーインターフェース
- モバイル端末対応
- GNU GPL-3.0ライセンスの下、オープンソースで自由に配布可能
- 単一HTMLファイルで動作する
- HTMLファイル内に、事前にリストを埋め込むことが可能
- アクセス解析を行うための Google Analytics のコードを埋め込み(不要な場合はコードを削除してください。<title>タグの直下に記述されています。)

## とりあえず使ってみる

以下のリンクを開いてください:

[Address Mapper with GSI](https://ysys-7.github.io/Address-Mapper-with-GSI/AMwG.html)

## リスト埋め込み版のデモ

以下のリンクを開いてください:

[Address Mapper with GSI embedded_demo](https://ysys-7.github.io/Address-Mapper-with-GSI/AMwG_embedded_demo.html)

## インストール方法

AMwG をローカルで使用するには、以下の手順に従ってください:

1. リポジトリをクローンする:
   
   ```sh
   git clone https://github.com/ysys-7/Address-Mapper-with-GSI.git
   ```

2. プロジェクト・ディレクトリに移動する:
   
   ```sh
   cd Address-Mapper-with-GSI
   ```

3. ウェブブラウザで`AMwG.html`を開く。

## 使用方法

1.施設名と住所のリストを半角カンマまたはタブで区切ってテキストエリアに入力します。

例:

```plaintext
東京都庁,東京都新宿区西新宿２丁目８−１
大阪城,大阪府大阪市中央区大阪城１−１
```

2. 「地図にプロット」ボタンをクリックすると、地図上に住所がプロットされます。

3. 「リセット」ボタンでページを再読み込みし、地図を消去する。

4. CSVファイル（Shift-JISエンコーディング）をインポートして住所をプロットすることもできます。

## FAQ

**Q: 住所を入力しても地図にプロットされません。**

A: 住所が正確に入力されていることを確認してください。また、施設名や住所に誤りがないかチェックしてください。施設名と住所の区切りが誤って全角カンマになっていないかチェックしてください。

**Q: CSVインポートがうまくいきません。**

A: CSVファイルのエンコーディングがShift-JISであることを確認してください。他のエンコーディング形式では動作しない可能性があります。

**Q: 地図上の位置が少しずれています。**

A: これはジオコーディングの誤差によるものである可能性があります。完全な精度を保証することは難しい場合がありますが、使用目的によっては許容範囲内であることをご確認ください。

## サポートとフィードバック

このプロジェクトはオープンソースであり、限られた時間の中で開発されています。バグ報告や機能リクエストについては、以下の方法でコミュニティと交流してください：

**Discussions**: 使用方法についての質問や他のユーザーとの議論を希望する場合は、[GitHub Discussions](https://github.com/ysys-7/Address-Mapper-with-GSI/discussions)をご利用ください。

## プルリクエスト

- プルリクエストは受け付けていません。これは、開発プロセスを管理しやすくし、私の個人的なスケジュールに合わせてアップデートが行われるようにするためです。
- 提案やフィードバックがある場合は、「Discussions」タブで意見を交換してください。私はこれを定期的に確認し、将来のアップデートのために検討します。

## 地理院地図の利用規約

本プロジェクト AMwG は、地理院地図および国土地理院のジオコーディングサービスを使用しています。利用規約については、以下のリンクを参照してください。

- [地理院地図利用規約](https://www.gsi.go.jp/kikakuchousei/kikakuchousei40182.html)
- 出典：[地理院地図](https://maps.gsi.go.jp)

## ライセンス

AMwGはGNU General Public License v3.0で配布されています。詳しくはLICENSEファイルをご覧ください。

## 原作者

Yossy (ysys-7)によって作成されました。詳細は[GitHub Repository](https://github.com/ysys-7/Address-Mapper-with-GSI)をご覧ください。
