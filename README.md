# yt-dlpGUI

This is the Japanese version of the README. For the English version, click here → [en](README.en.md)

## 概要
yt-dlpをGUIで使いやすくしたやつです。  
私が使うために作られたやつをいい感じにいい感じにしたやつです。

## 動作に必要なソフトウェア
- ffmpeg

> Windows環境でのインストール
> ```bash:ターミナル
> winget install Gyan.FFmpeg
> ```

## 主な機能
### 検索機能
URLを入れなくても検索ワードを入れると一番上の結果をダウンロードします。

### 形式・品質の選択
形式はmp4,mp3,サムネイルから選ぶことができます。mp4はたまにmkv形式で落とされる時があります。(修正予定)  
品質はmp4の場合、自動,144pから1080pまで選択可能。mp3の場合は自動,128kbpsから320kbpsまで4段階で選択可能です。

### プレイリスト云々
プレイリストのタイトルでフォルダを作成してその中に保存したり、  
ファイル名にプレイリストのインデックスをファイル名に追加したりってのができます。  
プレイリストをダウンロードするときにお使いください。

### サムネイルを追加
ファイルにサムネイルを埋め込んでくれます。

### Cookieの選択
cookies.txtなどの認証情報の入ったtxtファイルを選択してログインが必要な動画をダウンロードできるようになります。

## スクリーンショット

![image](https://github.com/user-attachments/assets/41a929f1-b9e3-497f-afb4-3335e6de8198)

![image](https://github.com/user-attachments/assets/239eef17-f7b3-4133-89bb-ff72e0d44a2e)

## 自分でビルド
pyinstallerを使いビルドできます。

このリポジトリをクローンしてカレントディレクトリを移動、そこで
```bash:
pyinstaller yt-dlpGUI.spec
```

を実行してください。  
`/dist`に保存されます。

## そのほかのOSでの動作
macOSで動作をすることを確認しています。  
```bash
python main.py
```
で動作させることが可能です。Linuxでは未検証です。
