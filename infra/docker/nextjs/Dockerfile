# ベースイメージ
FROM node:21-alpine3.18

# 作業ディレクトリを設定
WORKDIR /client

# package.json と package-lock.json をコピーして依存関係をインストール
COPY client/package*.json ./

# RUN npm install

# アプリケーションのソースコードをコピー
COPY client/ ./

# アプリケーションをビルド
RUN npm install

# ポート3000を公開
EXPOSE 3000

# アプリケーションを起動
CMD ["npm", "run", "dev"]