# AWS CLIインストール

> http://qiita.com/yuyj109/items/3163a84480da4c8f402c

MAC OSなので

~~~
pip install awscli
~~~

# AWS CLI設定
~~~
aws configure
~~~
IAMユーザのアクセスキー、シークレットキーを設定する。またリージョンを指定する

設定確認
~~~
aws configure list
~~~

## コマンド補完設定
下記の記載を~/.zshrcに追加

~~~
source /usr/local/bin/aws_zsh_completer.sh
~~~
