# Fcitx5

## 中文输入法

<tabs>
<tab title="Arch/Manjaro">
<code-block language="bash">
sudo pacman -Sy zsh git curl wget vim mpv vlc ffmpeg base-devel
</code-block>
</tab>
<tab title="Debain/Ubuntu">
<code-block language="bash">
sudo pacman -Sy zsh git curl wget vim mpv vlc ffmpeg base-devel
</code-block>
</tab>
</tabs>

打开 tweak 软件， 将 fcitx5 添加到开机自启动

使用命令 fcitx5 启动 Fcitx5 输入法

打开 fcitx5-config 软件，将 PinYIn 添加到输入法分组

重启系统生效

> 如果仍无法使用Fcitx5输入法，执行以下命令，重启系统

```Bash
sudo tee -a /etc/environment <<EOF
GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx
INPUT_METHOD=fcitx
SDL_IM_MODULE=fcitx
GLFW_IM_MODULE=ibus
EOF
```
