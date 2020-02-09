FROM python:3  # image名にpython3実行環境のイメージを指定
ENV PYTHONUNBUFFERED 1 # pythonの標準出力をバッファにため込まないための環境変数設定
RUN mkdir /service  # serviceディレクトリを作成
WORKDIR /service # serviceディレクトリに移動
COPY requirements.txt /service/  # requirements.txt(事前に作成)をserviceディレクトリに置く
RUN pip install -r requirements.txt # pip  installでパッケージをインストール
COPY . /service/ # buildコンテキストの内容を全て/service内に置く