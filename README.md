# zone-to-doc
以下の略形式の bind （zoneファイル）を markdown 形式に出力する。

```
$TTL 86400
@       IN  SOA  ns01.example.home. root@example.home. (
        2022121904  ;Serial
        3600        ;Refresh
        1800        ;Retry
        604800      ;Expire
        86400       ;Minimum TTL
)

@              IN  NS      ns01.example.home.
@              IN  A       192.168.1.101
ns01           IN  A       192.168.1.101

hoge           IN  A       192.168.1.10
fuga           IN  CNAME   hoge.example.home.
```
