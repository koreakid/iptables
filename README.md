该脚本非本人编码，乃引用arloor大佬的脚本。此为备份作用。如需详细了解，请到大佬的github：https://github.com/arloor/iptablesUtils ，再次感谢大佬出的脚本。
非常实用

## 用法

```shell
wget -qO natcfg.sh http://www.arloor.com/sh/iptablesUtils/natcfg.sh && bash natcfg.sh
```

或

```
wget -qO natcfg.sh https://raw.githubusercontent.com/koreakid/iptables/master/natcfg.sh && bash natcfg.sh
```

输出如下：

```
用途: 便捷的设置iptables端口转发
注意1: 到域名的转发规则在添加后需要等待2分钟才会生效，且在机器重启后仍然有效
注意2: 到IP的转发规则在重启后会失效，这是iptables的特性

你要做什么呢（请输入数字）？Ctrl+C 退出本脚本
1) 增加到域名的转发      3) 增加到IP的转发        5) 列出所有到域名的转发
2) 删除到域名的转发      4) 删除到IP的转发        6) 查看iptables转发规则
#? 
```

此时按照需要，输入1-6中的任意数字，然后按照提示即可

## trojan转发

总是有人说，不能转发trojan，这么说的人大部分是证书配置不对。最简单的解决方案是：客户端选择不验证证书。复杂一点是自己把证书和中转机的域名搭配好。

小白记住一句话就好：客户端不验证证书。

