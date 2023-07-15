# Upgrade Packages Playbook Description

更新主机中安装的软件。在软件被更新后，重启主机使更新生效。

示例：
-----

在 `hosts` inventory 中指定主机，例如：

```ini
[nodes]
192.168.1.10
192.168.1.20
```

执行命令：

```bash
ansible-playbook playbook.yaml
```

License
-------

BSD

Author
------------------

作者: 魏文第

欢迎关注公众号：魏文第
