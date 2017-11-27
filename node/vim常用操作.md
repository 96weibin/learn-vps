# vim常用操作

## 三种模式

- 命令模式(Command mode)
- 插入模式(Insert mode)

```vim
i
```

- 底线命令模式(Last line mode)

```vim
：
```

- 命令模式

>用户刚刚启动 vim 就进入的是命令模式 此状态下键入的 会被当做 vim 命令

- i   切换到插模式
- dd  删除一行
- [num]dd   删除多行
- esc + u 就撤销一次
- shift + $ 切换到行尾
- esc + :wq 或 shift + zz 或 ZZ 储存后离开

##　修改主机名字

```vim
  sudo vim/etc/hosts
```

### 重启生效

```vim
  sudo vim/etc/reboot
```

## 查看当前发行版可用的shell

```vim
  cat /etc/shells
```

## 更换主题

```vim
  vim ~/.zshrc
```

-修改[](https://camo.githubusercontent.com/8ba661edfcfdfb6bf922369205801708af0815aa/687474703a2f2f6d642e736875646f6e672e77616e672f323031372d31312d32372d31342d34322d32362e706e67)

## 应用主题

```vim
  source ~/.zshrc
```

## 用户操作

- 添加用户

>useradd [name];

- 创建用户家目录

>mkdir -p /home/[name];

- 给用户家命令

>chown -R [name]:[name] /home/[name];

- 授权于拥堵sudo权限

>gpasswd -a [name] sudo

- 设置用户密码

>passwd [name];

usermod -s /bin/bash [name]

## 文件操作

- 查看文件内容 

>cat;
