# Address Mapper with OSM (AMwO)

Address Mapper with OSM (AMwO)は、OpenStreetMapを使って地図上に住所をプロットできるウェブベースのツールです。ユーザーフレンドリーで高機能に設計されており、自治体事業や街づくりなど様々な用途に最適です。

## 特徴

- OpenStreetMapを使って複数の住所を地図上にプロット
- 国土地理院のジオエンコーディングサービスを使用
- CSVインポート機能（Shift-JISエンコーディングのみ）
- プロットされたすべての場所に合うように、地図のズームを自動調整
- シンプルで直感的なユーザーインターフェース
- GNU GPL-3.0ライセンスの下、オープンソースで自由に配布可能

## インストール方法

Address Mapper with OSM をローカルで使用するには、以下の手順に従ってください:

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

A: 住所が正確に入力されていることを確認してください。また、施設名や住所に誤りがないかチェックしてください。

**Q: CSVインポートがうまくいきません。**

A: CSVファイルのエンコーディングがShift-JISであることを確認してください。他のエンコーディング形式では動作しない可能性があります。

## サポートとフィードバック

このプロジェクトはオープンソースであり、限られた時間の中で開発されています。バグ報告や機能リクエストについては、以下の方法でコミュニティと交流してください：

**Discussions**: 使用方法についての質問や他のユーザーとの議論を希望する場合は、[GitHub Discussions](https://github.com/ysys-7/Address-Mapper-with-OSM/discussions)をご利用ください。

## ライセンス

Address Mapper with OSM (AMwO)はGNU General Public License v3.0で配布されています。詳しくはLICENSEファイルをご覧ください。

## 原作者

Yossy (ysys-7)によって作成されました。詳細はGitHub Repositoryをご覧ください。 https://github.com/ysys-7/Address-Mapper-with-OSM
