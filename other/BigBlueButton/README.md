# BigBlueButton

## 安装

> 参考：
>
> * [bbb 开发文档](https://bigbluebutton.org/developers/)
> * [bbb-install](https://github.com/bigbluebutton/bbb-install/tree/v2.7.x-release)

### 手动上传证书

域名 `bbb.vfanlee.eu.org`，证书放在 `/local/certs/`，`crt` 改名 `fullchain.pem`，`key` 改名 `privkey.pem`。

```sh
wget -qO- https://raw.githubusercontent.com/bigbluebutton/bbb-install/v2.7.x-release/bbb-install.sh | bash -s -- -w -v focal-270 -s bbb.vfanlee.eu.org -g -d -t ABCD:soTTTMk0LcWMu4dZViFh9W4maGqzs4zEzv3sWUL3Lo
```
