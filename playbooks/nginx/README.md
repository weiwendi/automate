# Deploy Nginx Playbook Description

自动化部署 Nginx。

示例：
-----

在 `hosts` inventory 中指定主机名。

Ansible 控制节点能够通过主机名登录远程主机，可以通过 DNS 服务或者 `/etc/hosts` 文件实现。

例如：

```ini
[lb]
lb1.server.aiops.red
lb2.server.aiops.red
```

Ansible 控制节点 hosts 文件：

```bash
cat /etc/hosts
# lb
10.211.55.56  lb1.server.aiops.red
10.211.55.57  lb2.server.aiops.red
```

执行命令：

```bash
ansible-playbook -i ./hosts playbook.yaml
```

详细内容请参考 **魏文第** 公众号文章 [Linux 9 自动化部署 Keepalived + Nginx 高可用负载均衡器](https://mp.weixin.qq.com/s?__biz=Mzk0MDAwOTUwNQ==&mid=2247484951&idx=1&sn=e7709648652bc741f1ad7be609aa60f7&chksm=c2e97759f59efe4f2b264fc699cbc0a8aae28c1d2b48c1a3b75e9ae28659147bac4e525189d2&token=1636185424&lang=zh_CN#rd)。

License
-------

BSD

Author
------------------

作者: 魏文第

欢迎关注公众号：魏文第
