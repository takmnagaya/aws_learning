# EC2の環境構築をAWS CLIで実行する

## 公開鍵、秘密鍵キーペアの作成
~~~
aws ec2 create-key-pair --key-name my-keypair-from-cli
~~~

~~~
(実行結果)
{
    "KeyMaterial": "-----BEGIN RSA PRIVATE KEY-----\nMIIjB....DHJPYwUg==\n-----END RSA PRIVATE KEY-----", 
    "KeyName": "my-keypair-from-cli", 
    "KeyFingerprint": "8e:5a:df:3a:02:73:89:1b:ec:7d:5a:1e:5c:fa:62:a1:9e:11:ba:bd"
}
~~~

`-----BEGIN RSA PRIVATE KEY-----...-----END RSA PRIVATE KEY-----`の部分を秘密鍵としてローカルに保持しておけば、
このキーペアを使ったEC2を立ち上げることで、SSHで接続できる。
