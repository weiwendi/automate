# Sudoers Playbook Description

自动化配置普通用户免密执行 **sudo** 命令。

示例：
-----

在 `hosts` inventory 中指定主机，例如：

```ini
[nodes]
192.168.1.10
192.168.1.20
```

`playbook.yaml` 示例中为 *aiops* 用户设置免密执行 **sudo** 命令，可以通过 `sudouser` 变量将其修改为实际使用的用户。

执行命令：

```bash
ansible-playbook playbook.yaml -K
```

非 *root* 用户下执行此 Playbook 时，需要通过 **-K** 选项提供 **sudo** 权限。

License
-------

BSD

Author
------

作者: 魏文第

欢迎关注公众号：魏文第
