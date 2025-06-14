# 常用工具


## 更新升级

<tabs>
<tab title="Arch">
<code-block lang="bash">
sudo pacman -Syu
</code-block>
</tab>
<tab title="Ubuntu24.04">
<code-block lang="bash">
# 更新软件源
sudo apt update
# 升级软件
sudo apt upgrade -y
</code-block>
</tab>
</tabs>

## 安装工具

<tabs>
<tab title="Arch/Manjaro">
<code-block lang="bash">
sudo pacman -Sy zsh git curl wget vim mpv vlc ffmpeg base-devel
</code-block>
</tab>
<tab title="Ubuntu24.04">
<code-block lang="bash">
sudo apt install -y curl wget zsh git vim
</code-block>
</tab>
</tabs>

## OhMyZsh

```Bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Git配置

```Bash
# 设置默认分之为 main
git config --global init.defaultBranch main

# 配置用户名
git config --global user.name "demo"

# 配置用户邮箱
git config --global user.email "demodeom@example.com"
```