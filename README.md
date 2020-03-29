[![GitHub issues](https://img.shields.io/github/issues/0ta2/mysql_role)](https://github.com/0ta2/mysql_role/issues)
[![GitHub stars](https://img.shields.io/github/stars/0ta2/mysql_role)](https://github.com/0ta2/mysql_role/stargazers)
![GitHub Actions](https://github.com/0ta2/mysql_role/workflows/Molecule%20Test/badge.svg)

mysql_role
=========

PHPをインストールするためのロールです。

Requirements
------------

特になし。

Role Variables
--------------

|            変数名             |      デフォルト       | タイプ  |                                         説明                                          |
| ----------------------------- | --------------------- | ------- | ------------------------------------------------------------------------------------- |
| mysql_community_enable        | false                 | boolean | OSデフォルトではなく、MySQL Community をインストールする場合は、true にしてください。 |
| mysql_root_password           | passwordPASSWORD@999  | string  | MySQLのパスワードを指定                                                               |
| default_authentication_plugin | mysql_native_password | string  | パスワードの認証方式を指定します。                                                    |

Dependencies
------------

特になし

Example Playbook
----------------

```
---
    - hosts: servers
      roles:
         - { role: 0ta2.mysql_role }
```

License
-------

![GitHub](https://img.shields.io/github/license/0ta2/mysql_role)
