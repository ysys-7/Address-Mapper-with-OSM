# Address Mapper with OSM (AMwO)

Address Mapper with OSM (AMwO)は、OpenStreetMapを利用して住所を地図上にプロットできるウェブベースのツールです。ユーザーフレンドリーで高機能に設計されており、自治体事業や街づくりなど様々な用途に活用できます。AMwOはGNU General Public License v3.0の下で配布されており、自由にカスタマイズが可能です。

## 開発の経緯

厚生労働省のサイトで労災指定医療機関を検索した際、テキストで羅列させるという、とってもユーザーフレンドリーな設計だったので、このツールを作成しました。このツールを使えば、施設名と住所から簡単に地図上にプロットし、視覚的に確認できるようになります。

## 特徴

- OpenStreetMapを使って複数の住所を地図上にプロット
- 国土地理院のジオエンコーディングサービスを使用
- CSVインポート機能（Shift-JISエンコーディングのみ）
- プロットされたすべての場所に合うように、地図のズームを自動調整
- シンプルで直感的なユーザーインターフェース
- モバイル端末対応
- GNU GPL-3.0ライセンスの下、オープンソースで自由に配布可能
- htmlファイル内に、事前にリストを埋め込むことが可能

## とりあえず使ってみる

以下のリンクを開いてください:

[Address Mapper with OSM](https://ysys-7.github.io/Address-Mapper-with-OSM/AMwO.html)

## リスト埋め込み版のデモ

[Address Mapper with OSM](https://ysys-7.github.io/Address-Mapper-with-OSM/AMwO_embedded_demo.html)

## インストール方法

AMwO をローカルで使用するには、以下の手順に従ってください:

1. リポジトリをクローンする:
   
   ```sh
   git clone https://github.com/ysys-7/Address-Mapper-with-OSM.git
   ```

2. プロジェクト・ディレクトリに移動する:
   
   ```sh
   cd Address-Mapper-with-OSM
   ```

3. ウェブブラウザで`AMwO.html`を開く。

## 使用方法

1.施設名と住所のリストをカンマまたはタブで区切ってテキストエリアに入力します。

例:

```plaintext
東京都庁,東京都新宿区西新宿２丁目８−１
大阪城,大阪府大阪市中央区大阪城１−１
```

2. 地図にプロット」ボタンをクリックすると、地図上に住所がプロットされます。

3. リセット "ボタンでページを再読み込みし、地図を消去する。

4. オプションで、CSVファイル（Shift-JISエンコーディング）をインポートして住所をプロットすることもできます。

## FAQ

**Q: 住所を入力しても地図にプロットされません。**

A: 住所が正確に入力されていることを確認してください。また、施設名や住所に誤りがないかチェックしてください。施設名と住所の区切りが誤って全角カンマになっていないかチェックしてください。

**Q: CSVインポートがうまくいきません。**

A: CSVファイルのエンコーディングがShift-JISであることを確認してください。他のエンコーディング形式では動作しない可能性があります。

**Q: 地図上の位置が少しずれています。**

A: これはジオエンコーディングの小数点以下の誤差によるものである可能性があります。完全な精度を保証することは難しい場合がありますが、使用目的によっては許容範囲内であることをご確認ください。

## サポートとフィードバック

このプロジェクトはオープンソースであり、限られた時間の中で開発されています。バグ報告や機能リクエストについては、以下の方法でコミュニティと交流してください：

**Discussions**: 使用方法についての質問や他のユーザーとの議論を希望する場合は、[GitHub Discussions](https://github.com/ysys-7/Address-Mapper-with-OSM/discussions)をご利用ください。

## ライセンス

AMwOはGNU General Public License v3.0で配布されています。詳しくはLICENSEファイルをご覧ください。

## 原作者

Yossy (ysys-7)によって作成されました。詳細はGitHub Repositoryをご覧ください。 https://github.com/ysys-7/Address-Mapper-with-OSM
