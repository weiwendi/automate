# Authorized_key Playbook Description

将公钥添加到远程主机的指定用户，实现免密登录。

示例：
-----

在 `hosts` inventory 中添加要配置免密登录的主机 IP，例如：

```ini
[nodes]
192.168.1.10
192.168.1.20
```

`playbook.yaml` 中默认为 *aiops* 用户设置免密登录，可以将其修改为实际用户，并指定实际公钥文件。

执行命令：

```bash
ansible-playbook playbook.yaml -k
# or
ansible-playbook playbook.yaml -k -b -K
```

**-k** 选项提供远程主机上 *aiops* 用户的登录密码；**-b -K** 选项用于本地用于与远程用户不一致的情况。

License
-------

BSD

Author Information
------------------

Author: weiwendi
欢迎关注公众号：魏文第


