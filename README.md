lifecycle
=================

Handles server lifecycle management tasks.

OS Platform
-----------------

### Debian

- trixie
- bookworm

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `filesystem_symlink_dir`

ホームディレクトリに作成するシンボリックリンクの名前

#### `filesystem_symlink_src_dir`

シンボリックリンク元のベースディレクトリ

#### `filesystem_symlink_force`

シンボリックリンクを強制的に変更するか否か

#### `filesystem_symlink_exclude_users`

ホームディレクトリへのシンボリックリンクの作成を除外ユーザー

#### `package_update_cache`

パッケージキャッシュの更新をするかどうか

#### `package_update_upgrade`

インストール済みパッケージの更新をするかどうか

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: lifecycle
```

License
--------------

Apache License 2.0
