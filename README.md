# Ansible-Playbook

## Description

Centos7にNginx + PHP 7 + mariadb + Let's encrypt (certbot) + Wordpressの環境を構築するPlaybookです。

## Requirements.

### Host
- Ansible 2.2

### Client
- CentOS 7.3

## Usage

実行する前に、`playbook.yml`の

```yaml
vars:
    HostName: "YOUR_HOSTNAME_HERE" 
    mysql_root_password: "YOUR_PASS_HERE"
    mysql_db_password: "YOUR_PASS_HERE"
    Email: "YOUR_EMAIL_HERE"
```

この部分を編集してください。

```bash
$ ansible-playbook playbook.yml
```
