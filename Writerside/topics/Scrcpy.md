# Scrcpy

## Download Scrcpy

```bash
wget https://github.com/Genymobile/scrcpy/releases/download/v3.2/scrcpy-linux-x86_64-v3.2.tar.gz
```

## Download Icon

```bash
wget https://raw.githubusercontent.com/Genymobile/scrcpy/refs/heads/master/app/data/icon.ico
sudo mv icon.ico /opt/scrcpy/
````

## Install

```Bash

tar -xvf scrcpy-linux-x86_64-v3.2.tar.gz && rm scrcpy-linux-x86_64-v3.2.tar.gz

sudo mv scrcpy-linux-x86_64-v3.2 /opt/scrcpy
```

## Create Desktop Icon



```bash
vim ~/.local/share/applications/scrcpy.desktop
```


内容如下

```
[Desktop Entry]
Version=1.0
Type=Application
Name=Scrcpy
Comment=Android screen mirroring
Exec=/opt/scrcpy/scrcpy
Icon=/opt/scrcpy/icon.ico
Terminal=false
Categories=Utility;
```

## 完整脚本


```bash
# 下载 scrcpy
wget https://github.com/Genymobile/scrcpy/releases/download/v3.2/scrcpy-linux-x86_64-v3.2.tar.gz

# 解压并删除安装包
tar -xvf scrcpy-linux-x86_64-v3.2.tar.gz && rm scrcpy-linux-x86_64-v3.2.tar.gz

# 将软件安装到 /opt 目录
sudo mv scrcpy-linux-x86_64-v3.2 /opt/scrcpy

# 创建快捷方式
vim ~/.local/share/applications/scrcpy.desktop

cat > ~/.local/share/applications/scrcpy.desktop <<'EOF'
[Desktop Entry]
Version=1.0
Type=Application
Name=Scrcpy
Comment=Android screen mirroring
Exec=/opt/scrcpy/scrcpy
Icon=/opt/scrcpy/icon.ico
Terminal=false
Categories=Utility;
EOF
```

