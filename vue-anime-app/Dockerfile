# ベースイメージとして公式のNode.jsイメージを使用
FROM node:16-alpine

# 作業ディレクトリを設定
WORKDIR /app

# package.jsonとpackage-lock.jsonをコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm install

# ソースコードをコピー
COPY . .

# 環境変数を設定
ENV HOST=0.0.0.0

# コンテナ起動時にアプリを起動
CMD ["npm", "run", "dev"]

# アプリが使用するポートを指定
EXPOSE 8080
