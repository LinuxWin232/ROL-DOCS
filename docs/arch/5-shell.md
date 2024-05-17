
# Shell 美化

您好！<br>
如果您觉得您的终端太难看了，可以美化一下！<br>
由于oh-my-zsh太慢了，所以这期教程使用zim作为框架。
如果您没有安装zsh，请先```sudo pacman -S zsh```。
### 1. 安装zim
```shell
curl -fsSL https://raw.githubusercontent.com/zimfw/install/master/install.zsh | zsh
```
### 2. 编辑配置文件
```shell
nano ~/.zimrc
```
### 3. 添加powerlevel10k模块并安装
```shell
zmodule romkatv/powerlevel10k
# CTRL+X Y ENTER
zimfw install
```
### 4. 切换默认shell并重启
```shell
sudo nano /etc/passwd
# 修改{yourname:x:1000:1000::/home/username:}这一行把/usr/bin/bash改成/usr/bin/zsh
# CTRL+X Y ENTER
reboot
```
下次启动zsh时会让您配置powerlevel10k。请按照自己需求选择。

## 字体
powerlevel10k中有很多图标无法显示，可以按照以下方法解决：
### 1. 安装字体
```shell
sudo pacman -S ttf-jetbrains-mono-nerd
```
### 2. 切换终端默认字体
**重要信息!**
由于大多数人的终端都不一样，所以这里只提供konsole的方法。

```shell
# 右键点击 - 编辑当前方案 - 外观
# 字体(选择) - 选择JetBrainsMono Nerd Font(不要选MONO!!) - 确定 - 确定
```
在这之后，您就可以使用ZSH了。