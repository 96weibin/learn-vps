# linux 操作

## 安装软件

  >apt-get  *Advanced Package Tool 先进的打包工具*

```vim
  apt-get install [name] -y
  apt-get install git -y
```

## 查看系统信息

```vim
  cat /etc/issue
```

## 更新源码包的仓库

```vim
  apt-get update -y
```

## 安装zshell

```vim
  apt-get install zsh git curl -y
```

- 两种方法 选一种即可

```vim
  sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"


  sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## 切换用户

- 添加用户
        因为默默认的 root 权限过大  一般都通过 linux 是支持多人的  所以 要可以分出一些只有部分功能的 用户

```vim
  adduser [name]
```

- 添加用户到sudo组
      sudo用户组就是 一些权限较小 的用户群组

```vim
  adduser [name] sudo
```

- 切换到这个用户

```vim
  su - [name]
```
