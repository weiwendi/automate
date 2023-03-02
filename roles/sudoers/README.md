# Sudoers Role Description

自动化配置普通用户免密执行 **sudo** 命令。

## 要求

执行本 Role 需要 *root* 用户权限，或具有 **sudo** 权限。

## 角色变量

在 Role 中，用到了 `sudouser` 变量，该变量的值是将要配置的免密执行 **sudo** 的用户名。

示例：

```yaml
sudouser: aiops
```

License
-------

BSD

作者信息
------------------

作者: 魏文第
欢迎关注公众号：魏文第
