# Dockerセットアップ手順書

- [Dockerセットアップ手順書](#docker%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%83%E3%83%97%E6%89%8B%E9%A0%86%E6%9B%B8)
	- [前提条件](#%E5%89%8D%E6%8F%90%E6%9D%A1%E4%BB%B6)
		- [OS](#os)
		- [仮想化ハードウェア拡張](#%E4%BB%AE%E6%83%B3%E5%8C%96%E3%83%8F%E3%83%BC%E3%83%89%E3%82%A6%E3%82%A7%E3%82%A2%E6%8B%A1%E5%BC%B5)
	- [Docker Toolboxインストール](#docker-toolbox%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)

## 前提条件

### OS

Windosw 10 Homeで確認した

### 仮想化ハードウェア拡張

仮想化ハードウェア拡張が有効になっていることを確認する

1. タスクマネージャーを起動
1. **詳細表示**にする
1. **パフォーマンス**タブを表示
1. **CPU**の**仮想化**が有効になっていることを確認する

無効の場合はBIOSを起動して**Intel(R) Virtualization Technology**を有効にする  
CPU、マザーボードによって微妙に違うので詳しくはググる

## Docker Toolboxインストール

1. [公式サイト](https://docs.docker.com/toolbox/toolbox_install_windows/)の**Get Docker Toolbox for Windows**からインストーラーをダウンロード
1. インストーラーを実行（チェックボックスは理由がなければデフォルトでOK）
1. デスクトップ、もしくはスタートメニューから**Docker Quickstart Terminal**を実行
1. クジラが表示されたら`docker run hello-world`を実行
1. `Hello from Docker!`が表示されればインストール完了
