# Open Firewall Role Description

在托管节点开启指定的端口。

## 要求

需要具有 **sudo** 权限的普通用户，或 *root* 用户。

## 使用说明

在 `defaults/main.yml` 文件中定义了 `open_ports` 变量，该变量为列表类型：

```yaml
---
# defaults file for firewalld
#
open_ports:
  # - 80/tcp
  # - 443/tcp
```

把需要开启的端口及端口协议类型，按示例 (- 80/tcp) 填写。

License
-------

BSD

Author
------------------

作者: 魏文第

欢迎关注公众号：魏文第
