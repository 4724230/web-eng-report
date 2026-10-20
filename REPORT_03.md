# 第3回 Webエンジニアリング演習 レポート
## 学籍番号
4724230
## イメージとコンテナの違い
イメージは、実行に必要なものをまとめた読み取り専用のパッケージ
コンテナは、そのイメージをもとに作られた実行中の環境の事である。
## Dockerfileの各行の役割
FROM nginx:1.29-alpine　役割：• ベースとなるDockerイメージを指定する。
COPY index.html /usr/share/nginx/html/index.html　役割：ローカルのファイルをコンテナ内にコピーする。
## 動作確認
HTMLの見出しを「Docker Composeで配信中」に変更した。

docker compose ps の実行結果
NAME                   IMAGE                                                                     COMMAND                  SERVICE   CREATED          STATUS          PORTS
web-eng-report-web-1   sha256:2c453f641c6b7091e176b38c974c49b66462023d622bcbb9d8866b27bb984657   "/docker-entrypoint.…"   web       21 minutes ago   Up 21 minutes   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp