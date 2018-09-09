# Webサーバー構築手順

- [Webサーバー構築手順](#web%E3%82%B5%E3%83%BC%E3%83%90%E3%83%BC%E6%A7%8B%E7%AF%89%E6%89%8B%E9%A0%86)
	- [前提条件](#%E5%89%8D%E6%8F%90%E6%9D%A1%E4%BB%B6)
	- [コンテナrun](#%E3%82%B3%E3%83%B3%E3%83%86%E3%83%8Arun)
	- [動作確認](#%E5%8B%95%E4%BD%9C%E7%A2%BA%E8%AA%8D)

## 前提条件

[RaspberryPiセットアップ手順書](https://github.com/pon3939/Manual/blob/master/RaspberryPi/初期設定/RaspberryPiセットアップ手順書.md)の作業を終えていること

## コンテナrun

```bash
docker run -d --restart=always -p 80:80 --name httpd hypriot/rpi-busybox-httpd
```

## 動作確認

下記を実行して、ブラウザで表示されればOK

```bash
docker exec -it httpd busybox ash
vi /www/test.html # 適当なファイルを作成
```
