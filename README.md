# SS2LF • SiteShield to LinodeFirewall

Akamai Site Shiledの更新をGithub Actionsを利用して、Linode Firewallへ自動的に適用するワークフローです。

手動の手順は以下を参照。

https://community.akamai.com/customers/s/article/JapanUserGroupSiteShield20190627090957?language=en_US

# Setup

利用する際には、Actions secretsを設定します。

- AKAMAI_CREDENTIALS
- MAP_ID
- LINODE_CLI_TOKEN
- FIREWALL_ID


```
# AKAMAI_CREDENTIALS

[default]
client_secret = 
host = akab-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx.luna.akamaiapis.net
access_token = xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
client_token = xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

# 取得方法

https://qiita.com/kabe-akam/items/499507d19220b44b4901
```

```
# MAP_ID

1111111

# Akamai CLIでの確認

akamai site-shield --section default list-maps
```

```
# LINODE_CLI_TOKEN

xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

# 取得方法

https://www.linode.com/docs/guides/getting-started-with-the-linode-api/
```

```
# FIREWALL_ID

11111

# Linode CLIでの確認

linode-cli firewalls list
```

# License
The source code is licensed MIT. The website content is licensed CC BY 4.0,see LICENSE.
